#### Parser Content
```Java
{
Name = cef-carbonblack-workstation-locked
  Vendor = VMware
  Product = VMware Carbon Black App Control
  Lms = ArcSight
  DataType = "workstation-locked"
  TimeFormat = "epoch"
  Conditions = [ """|Carbon Black|Protection|""", """Event[00000007] Type[SessionLock]""" ]
  Fields = [
    """\Wrt=({time}\d+)""",
    """\Wdvc=({host}[a-fA-F:\d.]+)""",
    """\Wdvchost=({host}[\w\-.]+)""",
    """\Wdhost=(({domain}[^\\]+)\\+)?({dest_host}[^\\\s]+)""",
    """\Wdst=({dest_ip}[a-fA-F:\d.]+)""",
    """\Wduser=(({domain}[^\\]+)\\+)?({user}[^\\\s]+)""",
    """\WEvent\[({event_code}\d+)\]\s*Type\[Session"""
  ]
}
```