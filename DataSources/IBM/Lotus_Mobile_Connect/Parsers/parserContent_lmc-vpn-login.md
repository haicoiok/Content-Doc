#### Parser Content
```Java
{
Name = lmc-vpn-login
  Vendor = IBM
  Product = Lotus Mobile Connect
  Lms = Direct
  DataType = "vpn-login"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
  Conditions = [ """"action":"lmc_login_""", """"userID":"""", """"srcIP":""" ]
  Fields = [
    """"@timestamp":"({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d\.\d+Z)""",
    """({host}[\w\-.]+)\s+\{"""",
    """"srcIP":\s*"({src_ip}[A-Fa-f:\d.]+)""",
    """"dstIP":"({dest_ip}[A-Fa-f:\d.]+)""",
    """"action":"({action}[^"]+)""",
    """"userID":"({user}[^"\s]+)""",
  ]
  DupFields = ["user->account"]
}
```