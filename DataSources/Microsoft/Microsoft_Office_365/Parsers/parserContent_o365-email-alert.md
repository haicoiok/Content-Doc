#### Parser Content
```Java
{
Name = o365-email-alert
  Vendor = Microsoft
  Product = Microsoft Office 365
  Lms = Syslog
  DataType = "dlp-email-alert"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
  Conditions = [ """O365 Messages logrhythm:""", """TS=""", """SESSID=""" ]
  Fields = [
    """exabeam_host=([^=]+@\s*)?({host}[\w\-.]+)""",
    """TS=({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)""",
    """RECIPIENT=({recipient}[^\s]+)""",
    """SENDER=({sender}[^\s]+)""",
    """DOMAIN=({external_domain}[^\s]+)""",
    """SIP=({src_ip}[a-fA-F\d.:]+)""",
    """DIP=({dest_ip}[a-fA-F\d.:]+)""",
    """SUBJECT=(|({subject}.+?))\s+\w+=""",
    """STATUS=({outcome}[^\s]+)""",
    """SIZE=({bytes}\d+)""",
    """SESSID=({message_id}[^\s]+)""",
  ]
}
```