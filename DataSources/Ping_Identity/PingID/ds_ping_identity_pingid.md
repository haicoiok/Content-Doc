Vendor: Ping Identity
=====================
Product: PingID
---------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  14   |   4    |     3      |      6      |    6    |

|                Use-Case                | Activity Types                                                                                                     | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | MITRE TTP                                                                       | Content                                                                                                |
|:--------------------------------------:| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [Other](../../../UseCases/uc_other.md) | <ul><li>Activity Time  and Type</li><li>Asset Logon and Access</li><li>Network zones and Location Access</li></ul> |  account-password-change<br> ↳ [cef-pingid-auth](Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-change-failed<br> ↳ [cef-pingid-auth](Parsers/parserContent_cef-pingid-auth.md)<br><br> account-password-reset<br> ↳ [cef-pingid-auth](Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-attempt<br> ↳ [cef-pingid-auth](Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-failed<br> ↳ [cef-pingid-auth](Parsers/parserContent_cef-pingid-auth.md)<br><br> authentication-successful<br> ↳ [cef-pingid-auth](Parsers/parserContent_cef-pingid-auth.md)<br> | T1078 - Valid Accounts<br>T1133 - External Remote Services<br>T1188 - T1188<br> | [<ul><li>14 Rules</li></ul><ul><li>4 Models</li></ul>](Rules_Models/r_m_ping_identity_pingid_Other.md) |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution | Persistence                                                                                                                                      | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     |              |        |