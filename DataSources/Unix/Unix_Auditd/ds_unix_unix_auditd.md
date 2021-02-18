Vendor: Unix
============
Product: Unix Auditd
--------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  96   |   21   |     14     |      7      |    7    |

|                Use-Case                | Activity Types                                                                                                                                                                                                                                                                                                                                                                 | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | MITRE TTP                                                                                                                                                                                                                                                                                                                                                                                  | Content                                                                                             |
|:--------------------------------------:| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| [Other](../../../UseCases/uc_other.md) | <ul><li>Activity Time  and Type</li><li>Asset Logon and Access</li><li>Credential Switch Activity</li><li>Critical System Activity</li><li>Endpoint Activity</li><li>Executives</li><li>Failed Logon and Account Lockout</li><li>Network zones and Location Access</li><li>Pass The Hash and Golden Ticket</li><li>Process Activity</li><li>Service Account Activity</li></ul> |  account-switch<br> ↳ [cef-unix-su-2](Parsers/parserContent_cef-unix-su-2.md)<br> ↳ [cef-unix-su-1](Parsers/parserContent_cef-unix-su-1.md)<br> ↳ [unix-account-switch-json](Parsers/parserContent_unix-account-switch-json.md)<br><br> app-activity-failed<br> ↳ [cef-unix-ssh-disconnect](Parsers/parserContent_cef-unix-ssh-disconnect.md)<br><br> failed-logon<br> ↳ [unix-ssh-login-failed-json](Parsers/parserContent_unix-ssh-login-failed-json.md)<br> ↳ [unix-ssh-login-failed-json-1](Parsers/parserContent_unix-ssh-login-failed-json-1.md)<br> ↳ [cef-unix-ssh-fail](Parsers/parserContent_cef-unix-ssh-fail.md)<br><br> local-logon<br> ↳ [cef-unix-local-logon](Parsers/parserContent_cef-unix-local-logon.md)<br> ↳ [cef-unix-local-logon-2](Parsers/parserContent_cef-unix-local-logon-2.md)<br> ↳ [cef-unix-local-logon-1](Parsers/parserContent_cef-unix-local-logon-1.md)<br><br> process-created<br> ↳ [cef-aix-process-created](Parsers/parserContent_cef-aix-process-created.md)<br><br> process-created-failed<br> ↳ [unix-process-creation-failure](Parsers/parserContent_unix-process-creation-failure.md)<br><br> remote-logon<br> ↳ [unix-ssh-login-json](Parsers/parserContent_unix-ssh-login-json.md)<br> | T1003 - OS Credential Dumping<br>T1021 - Remote Services<br>T1036 - Masquerading<br>T1068 - Exploitation for Privilege Escalation<br>T1075 - T1075<br>T1078 - Valid Accounts<br>T1097 - T1097<br>T1098 - Account Manipulation<br>T1110 - Brute Force<br>T1133 - External Remote Services<br>T1188 - T1188<br>T1204 - User Execution<br>T1208 - T1208<br>T1219 - Remote Access Software<br> | [<ul><li>96 Rules</li></ul><ul><li>21 Models</li></ul>](Rules_Models/r_m_unix_unix_auditd_Other.md) |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution                                                           | Persistence                                                                                                                                                                                                               | Privilege Escalation                                                                                                                                          | Defense Evasion                                                                                                                      | Credential Access                                                                                                                          | Discovery | Lateral Movement                                                     | Collection | Command and Control                                                         | Exfiltration | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | --------- | -------------------------------------------------------------------- | ---------- | --------------------------------------------------------------------------- | ------------ | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Account Manipulation](https://attack.mitre.org/techniques/T1098)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Exploitation for Privilege Escalation](https://attack.mitre.org/techniques/T1068)<br><br> | [Masquerading](https://attack.mitre.org/techniques/T1036)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [OS Credential Dumping](https://attack.mitre.org/techniques/T1003)<br><br>[Brute Force](https://attack.mitre.org/techniques/T1110)<br><br> |           | [Remote Services](https://attack.mitre.org/techniques/T1021)<br><br> |            | [Remote Access Software](https://attack.mitre.org/techniques/T1219)<br><br> |              |        |