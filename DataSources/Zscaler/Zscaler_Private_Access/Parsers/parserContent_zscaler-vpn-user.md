#### Parser Content
```Java
{
Name = zscaler-vpn-user
  Vendor = Zscaler
  Product = Zscaler Private Access
  Lms = Direct
  DataType = "vpn-user"
  TimeFormat = "MMM dd HH:mm:ss yyyy"
  Conditions = [ """ User Activity zpa-lss:""" ]
  Fields = [
    """exabeam_host=([^=]+@\s*)?({host}\S+)""",
    """\w+ ({time}\w+ \d+ \d\d:\d\d:\d\d \d\d\d\d) User Activity zpa-lss:([^,]*,){2}({session_id}[^,]+),({connection_id}[^,]+),([^,]*,){2}({connection_status}[^,]+),({protocol}[^,]+),[^,]*,({user_email}[^\s,]+),({src_port}\d+),({src_ip}[A-Fa-f:\d.]+)"""
  ]
}
```