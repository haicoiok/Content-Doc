#### Parser Content
```Java
{
Name = s-o365-dlp-alert
  Vendor = Microsoft
  Product = Windows Defender
  Lms = Splunk
  DataType = "dlp-alert"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
  Conditions = [ """"From":""", """"Workload":""", """"Actions":""", """"DLPRuleMatch"""" ]
  Fields = [
    """"CreationTime":\s*"({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)""",
    """exabeam_host=({host}[^\s]+)""",
    """"PolicyName":\s*"(|({alert_type}[^"]+))"(,|\})""",
    """"SensitiveInformation":\s*\[\{[^\}]*?"Location":\s*"(|({additional_info}[^"]+))"(,|\})""",
    """"Severity":\s*"({alert_severity}[^"]+)"""",
    """"IncidentId":\s*"({alert_id}[^"]+)"""",
    """"Actions":\s*\["({outcome}[^"]+)"""",
    """"RuleName":\s*"(|({alert_name}[^",\(]+?)\s*)("|\()""",
    """"FileName":\s*"(|({file_name}[^"]+))"(,|\})""",
    """"From":\s*"({user_email}[^@"]+?@[^@]+?)"""",
    """"To":\s*\[({target}[^\]]+?)\]"""
  ]
  DupFields = [ "user_email->user" ]
}
```