#### Parser Content
```Java
{
Name = s-mssql-database-query-al-xml
  Lms = Direct
  DataType = "database-query"
  Conditions = [ """>33205</EventID>""", """action_id:AL""" ]
  Fields = ${MicrosoftParserTemplates.s-mssql-database-query.Fields} [
    """\sserver_principal_name:({domain}[^\s]+)""",
    """\sserver_principal_name:(({domain}[^\\]+)\\)?({user}[^\s]+)\sserver_principal_sid""",
    """\sserver_principal_sid:({db_user_sid}[^\s]+)""",
  ]
}
```