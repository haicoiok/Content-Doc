#### Parser Content
```Java
{
Name = syslog-l7-app-activity-get
  Vendor = Kemp
  Product = Kemp LoadMaster
  Lms = Direct
  DataType = "app-activity"
  TimeFormat = "epoch"
  Conditions = [ """l7log:""" , "User ", """ requested GET """ ]
  Fields = [
    """exabeam_host=({host}[\w\-\.]+)""",
    """\s({host}[\w\-\.]+?)\s+\w+\d+\s+\-\s+l7log:""",
    """\d+log:\s*({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}):({dest_port}\d+):\s*\(({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}):({src_port}\d+)\)""",
    """\sUser\s*\'(({domain}[^']+)\\)?({user}[^']+)\'""",
    """\sUser\s*\'({user_email}[^\s@]+@[^\s@]+)\'""",
    """\sUser\s*\'({user}[^\s@]+@[^\s]+)\'""",
    """\srequested ({activity}GET) ({object}.+?)\s*$""",
  ]
}
```