#### Parser Content
```Java
{
Name = cef-salesforce-app-activity-27
  Vendor = Salesforce
  Product = Salesforce
  Lms = ArcSight
  DataType = "app-activity"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
  Conditions = [ """Action\=createdrole""", """Sales Cloud""" ]
  Fields = [
    """exabeam_host=([^=]+@\s*)?({host}\S+)""",  
    """CreatedDate\\=({time}\d\d\d\d\-\d\d\-\d\dT\d\d:\d\d:\d\d\.\d\d\dZ)"""
    """CreatedBy\.Username\\=({user_email}[^@]+@({email_domain}[^\s;]+))""",
    """suser=({user}.+?)\s+(\w+=|$)""",
    """suser=({user_email}[^@\s]+?@[^@\s]+)\s*(\w+=|$)""",
    """Action\\=({activity}[^;]+)""",
    """Display\\=({additional_info}.+?)\s*(\w+=|$)""",
    """Display\\=Created new role Field Service\s*\-\s*({object}.+?)\s+(\w+=|$)""",
    """({app}Sales Cloud)""",
  ]
}
```