#### Parser Content
```Java
{
Name = mariadb-alter
  Vendor = MariaDB
  Product = MariaDB
  Lms = Direct
  DataType = "database-update"
  TimeFormat = "yyyyMMdd HH:mm:ss"
  Conditions = [ """MariaDB:""","""ALTER""" ]
  Fields = [
    """MariaDB:\s({time}\d+\s\d\d:\d\d:\d\d)""",
    """\:\d{2}\,({host}[^\,]+)?\,({user}[^\,]+)?\,({src_ip}[^,]+)?,({connection_id}\d+)?\,({query_id}\d+)?\,({db_operation}\w+)?\,({database_name}[^\,]+)?\,({object}[^\,]+)?"""
  ]
}
```