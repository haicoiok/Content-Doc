#### Parser Content
```Java
{
Name = s-azure-storage-activity
  Vendor = Microsoft
  Product = Microsoft Azure
  Lms = Splunk
  DataType = "cloud-storage-access"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
  Conditions = [ """resourceProviderName":{"value":"Microsoft.Storage"""  ]
  Fields = [
    """exabeam_host=([^=]+@\s*)?({host}[^\s]+)""",
    """"resourceProviderName":\s*\{[^\}]*?"localizedValue":\s*"({service}[^"]+)"""",
    """"eventTimestamp":\s*"({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)""",
    """"operationName":\s*\{[^\}]*?"localizedValue":\s*"({activity}[^"]+)"""",
    """"caller":\s*"({user}[^"\s@]+)"""",
    """"caller":\s*"({user_email}[^"\s@]+@[^"\s@]+)"""",
    """"httpRequest":\s*\{[^\}]*?"clientIpAddress":\s*"({src_ip}[a-fA-F\d.:]+)""",
    """"tenantId":"({account_id}[^"]+)""",
    """"status":\{"value":"({outcome}[^"]+)""",
    """"resourceId".+?\/containers\/({bucket}[^\/"])""",
  ]
   DupFields = ["event_hub_namespace->host"]
}
```