#### Parser Content
```Java
{
Name = cef-incapsula-web-activity-2
  Vendor = Imperva
  Product = Incapsula
  Lms = Splunk
  DataType = "web-activity"
  TimeFormat = "epoch"
  Conditions = [ """CEF:""", """|Incapsula|SIEMintegration|""", """deviceExternalId""", """ ccode""" ]
  Fields = [
	"""exabeam_host=([^=]+@\s*)?({host}[\w\-.]+)""",
	"""sip\\=({dest_ip}\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})\s""",
	"""start\\=({time}\d+)""",
	"""src\\=({src_ip}\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})\s""",
	"""sourceServiceName\\=({web_domain}([^\s]+\.)?({top_domain}[^\s]+\.[^\s]+)?)\s""",
	"""act\\=({action}[A-Z_]+)\s""",		
	"""requestClientApplication\\=({user_agent}.+?)\s+(\w+\\=|$)""",
	"""cn1\\=({result_code}\d+)\s""",
	"""cpt\\=({src_port}\d+)\s""",
	"""spt\\=({dest_port}\d+)\s""",
	"""app\\=({protocol}[^|\s]+)\s""",
	"""request\\=({uri_path}[^\s]+)\s""",
	"""qstr\\=({uri_query}[^|]+)\\\\=""",
	"""in\\=({bytes}\d+|$)\s""",
	"""dproc\\=({browser}.+?)\s+(\w+\\=|$)"""
  ]

  DupFields = [ "uri_path ->full_url" ]
}
```