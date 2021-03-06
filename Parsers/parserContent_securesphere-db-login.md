#### Parser Content
```Java
{
Name = securesphere-db-login
  Vendor = Imperva
  Product = Imperva SecureSphere
  Lms = Direct
  DataType = "database-login"
  IsHVF = true
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ """Imperva |""", """operationname=Login""", """authenticated=True""" ]
  Fields = [
    """exabeam_host=({host}[\w\-.]+)""",
    """exabeam_time=({time}\d\d\d\d\-\d\d\-\d\d \d\d:\d\d:\d\d)""",
    """\ssrc=({src_ip}\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})""",
    """\sspt=({src_port}\d+)""",
    """\sdst=({dest_ip}\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})""",
    """\sdpt=({dest_port}\d+)""",
    """\sprotocol=({protocol}.*?)\s\w+=""",
    """\sservicename=({service_name}.*?)\s\w+=""",
    """\sservergroup=({server_group}[^\s]+)""",
    """\sappname=({app}.*?)\s\w+=""",
    """\sauthenticated=({outcome}\s\w+=)""",
    """\ssrchostname=({src_host}[^\s]+)""",
    """\sdbname=({db_name}[^\s]+)""",
    """\sschemaname=({db_schema}[^\s]+)"""
    """\sresponsesize=({response_size}.*?)\s\w+=""",
    """\sosuser=({os_user}[^\s]+])""",
    """\sduser=({db_user}[^\s]+)""", 
  ]
  DupFields = [ "db_user->account", "os_user->user" ]
}
```