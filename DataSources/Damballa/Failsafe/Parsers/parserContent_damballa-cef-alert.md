#### Parser Content
```Java
{
Name = damballa-cef-alert
  Vendor = Damballa
  Product = Failsafe
  Lms = ArcSight
  DataType = "alert"
  TimeFormat = "epoch"
  Conditions = [ "CEF:", """|Damballa|Failsafe""" ]
  Fields = [
    """exabeam_EventTime=({eventtime}\d+)""",
    """\|Damballa\|.+?\|.+?\|.+?\|({alert_name}[^\|]+?)\|""",
    """\|Damballa\|.+?\|.+?\|.+?\|.+?\|({alert_severity}[^\|]+)""",
    """\seventId=({alert_id}[^\s]+)""",
    """\srt=({time}\d+)""",
    """\ssrc=({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\sdst=({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\sshost=({src_host}[^\.\s]+)""",
    """\sdhost=({dest_host}[^\.\s]+)""",
    """\srequest=({malware_url}.+?)\s+\w+=""",
    """\sdvc=({host}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """\sdvchost=({host}[^\s]+)""",
    """\sreason=({alert_type}[^\s]+)"""
  ]
}
```