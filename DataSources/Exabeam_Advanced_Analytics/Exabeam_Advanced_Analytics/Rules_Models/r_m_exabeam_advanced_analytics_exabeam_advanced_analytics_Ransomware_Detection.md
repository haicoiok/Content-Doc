Vendor: Exabeam Advanced Analytics
==================================
### Product: [Exabeam Advanced Analytics](../ds_exabeam_advanced_analytics_exabeam_advanced_analytics.md)
### Use-Case: [Ransomware Detection](../../../../UseCases/uc_ransomware_detection.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   3   |   1    |     2      |      2      |    2    |

| Event Type   | Rules                                                                                                                                                                                                                                                                                                                                                | Models |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| app-activity | <b>T1078 - Valid Accounts</b><br> ↳ <b>Auth-Blacklist-Shost</b>: User authentication or login from a known blacklisted IP<br> ↳ <b>Auth-Ransomware-Shost</b>: User authentication or login from a known ransomware IP<br><br><b>T1090.003 - Proxy: Multi-hop Proxy</b><br> ↳ <b>Auth-Tor-Shost</b>: User authentication or login from a known TOR IP |        |
| app-login    | <b>T1078 - Valid Accounts</b><br> ↳ <b>Auth-Blacklist-Shost</b>: User authentication or login from a known blacklisted IP<br> ↳ <b>Auth-Ransomware-Shost</b>: User authentication or login from a known ransomware IP<br><br><b>T1090.003 - Proxy: Multi-hop Proxy</b><br> ↳ <b>Auth-Tor-Shost</b>: User authentication or login from a known TOR IP |        |