#### Parser Content
```Java
{
Name = n-forwarded-cef-dns-update
  Vendor = Microsoft
  Product = Microsoft Windows
  Lms = Direct
  DataType = "dhcp"
  TimeFormat = "epoch"
  Conditions = [ """|McAfee|ESM|""", """|272-32|""", """|Win_DHCP DNS dynamic update successful|""" ]
  Fields = [
    """exabeam_host=({host}[^\s]+)""",
    """\srt=({time}\d+)""",
    """\sshost=({dest_host}[^.\s]+)""",
    """\ssrc=({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
  ]
  DupFields = [ "dest_host->user" ]
}
```