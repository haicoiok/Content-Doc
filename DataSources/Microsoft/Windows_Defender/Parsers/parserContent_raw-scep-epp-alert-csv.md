#### Parser Content
```Java
{
Name = raw-scep-epp-alert-csv
  Vendor = Microsoft
  Product = Windows Defender
  Lms = Direct
  DataType = "alert"
  TimeFormat = "MMM dd yyyy HH:mma"
  Conditions = [ ",SystemCenterEndpointProtection" ]
  Fields = [
    """exabeam_host=(.+?@\s*)?({host}[^\s]+)""",
    """({time}\w+\s+\d+\s+\d\d\d\d\s+\d{1,2}:\d\d(AM|am|PM|pm))\,({alert_id}[^\,]+)\,({alert_name}[^\,]+)\,\w+\,({src_host}[^\,]+)\,[^,]+\,({additional_info}[^\,]+)\,(?:NA|({domain}[^\\]+))\\({user}[^\,]+)\,({alert_type}[^\,]+)\,({alert_severity}[^\,]+)\,SystemCenterEndpointProtection"""
  ]
}
```