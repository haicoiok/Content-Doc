#### Parser Content
```Java
{
Name = cef-skyformation-login-2
  Vendor = Cloud Application
  Product = Cloud Application
  Lms = ArcSight
  DataType = "app-login"
  TimeFormat = "epoch"
  Conditions = [ """|Skyformation|""", """"Action":"Login"""" ]
  Fields = [
    """exabeam_host=({host}[\w.\-]+)""",
    """\WdestinationServiceName=({app}.+?)(\s+\w+=|\s*$)""",
    """\Wend=({time}\d+)""",
    """\Wdproc=({process_name}.+?)(\s+\w+=|\s*$)""",
    """\Wfname=(?:({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|({dest_host}.+?))(\s+\w+=|\s*$)""",
    """\Wmsg=({additional_info}.+?)(\s+\w+=|\s*$)""",
    """\Wsrc=({src_ip}[a-fA-F\d.:]+)""",
    """\Wsuser=({user_email}[^@\s]+@({email_domain}[^@\s]+))""",
    """\Wsuser=({user_fullname}\w+(\s+\w+)+)""",
  ]
}
```