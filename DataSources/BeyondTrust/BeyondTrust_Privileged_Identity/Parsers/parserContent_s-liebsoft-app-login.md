#### Parser Content
```Java
{
Name = s-liebsoft-app-login
    Vendor = BeyondTrust
    Product = BeyondTrust Privileged Identity
    Lms = Splunk
    DataType = "app-login"
    TimeFormat = "yyyy-dd-MM'T'HH:mm:ss"
    Conditions = [ """sEventID="EVENT_ID_WEBAPP_LOGIN"""","""<Event"""]
    Fields = [
        """\d+:\d+:\d+\s+({host}[^\s]+)\s+<Event""",
        """dtPostTime="({time}\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2})""",
        """sOriginatingApplicationName="({app}[^"]+)""",
        """sIpAddress="({src_ip}[a-fA-F\d.:]+)""",
        """sLoginName="(({domain}[^"]+)\\)?({user}[^"]+)""",
        """sOriginatingSystem="({dest_host}[^"]+)"""
    ]
  }
```