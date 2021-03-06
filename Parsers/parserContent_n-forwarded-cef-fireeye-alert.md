#### Parser Content
```Java
{
Name = n-forwarded-cef-fireeye-alert
  Vendor = FireEye
  Product = FireEye Network Security (NX)
  Lms = NitroCefSyslog
  DataType = "alert"
  TimeFormat = "epoch"
  Conditions = [ "|McAfee|ESM", "|444-2835433003|" ]
  Fields = [ """\srt=({time}\d+)""",
    """\|McAfee\|ESM\|.+?\|.+?\|({alert_name}.+?)\|""",
    """\|McAfee\|ESM\|.+?\|.+?\|.+?\|({alert_severity}.+?)\|""",
    """\sdeviceTranslatedAddress=({host}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\sexternalId=({alert_id}\d+)""",
    """\sshost=({src_host}[^\s]+)""",
    """\ssrc=({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\sdst=({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\snitroObjectID=({alert_type}.+?)\s+nitroAttacker_IP""",
    """\snitroURL=({additional_info}[^\r\n]+)\s+"""
  ]
  SOAR {
    IncidentType = "malware"
    DupFields = ["time->startedDate", "vendor->source", "rawLog->sourceInfo", "alert_name->malwareName", "alert_id->sourceId", "alert_type->malwareCategory", "alert_severity->sourceSeverity", "src_host->malwareVictimHost", "dest_ip->malwareAttackerIp"]
    NameTemplate = """FireEye Alert ${alert_name} found"""
    ProjectName = "SOC"
    EntityFields = [
      {EntityType="device", Name="src_address", Fields=["src_ip->ip_address", "src_host->host_name"]}
```