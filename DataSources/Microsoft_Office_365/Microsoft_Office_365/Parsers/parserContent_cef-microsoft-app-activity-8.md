#### Parser Content
```Java
{
Name = cef-microsoft-app-activity-8
  Product = Microsoft Office 365
  Conditions= [ """CEF:""", """|Skyformation|SkyFormation Cloud Apps Security|""", """destinationServiceName=Office 365""", """|permissions-updated|""" ]
  Fields = ${MSParserTemplates.cef-microsoft-app-activity.Fields} [
    """sourceServiceName=({app}[^=]+?)\s+(\w+=|$)""",
  ]
}
```