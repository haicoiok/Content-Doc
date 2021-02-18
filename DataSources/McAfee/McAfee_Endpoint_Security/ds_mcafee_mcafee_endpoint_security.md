Vendor: McAfee
==============
Product: McAfee Endpoint Security
---------------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  34   |   12   |     7      |      6      |    6    |

|                Use-Case                | Activity Types                                                                                                                                                                                                                                                             | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | MITRE TTP                                                                                                                                                                                                                | Content                                                                                                            |
|:--------------------------------------:| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| [Other](../../../UseCases/uc_other.md) | <ul><li>Application Activity</li><li>Asset Logon and Access</li><li>Critical System Activity</li><li>Data Loss Prevention</li><li>Endpoint Activity</li><li>Executives</li><li>Network zones and Location Access</li><li>Process Activity</li><li>Security Alert</li></ul> |  failed-app-login<br> ↳ [cef-mcafee-skyhigh-failed-app-login](Parsers/parserContent_cef-mcafee-skyhigh-failed-app-login.md)<br><br> print-activity<br> ↳ [mcafee-dlp-print](Parsers/parserContent_mcafee-dlp-print.md)<br><br> process-alert<br> ↳ [s-mcafee-process-alert](Parsers/parserContent_s-mcafee-process-alert.md)<br> ↳ [cef-mcafee-process-alert](Parsers/parserContent_cef-mcafee-process-alert.md)<br><br> security-alert<br> ↳ [s-mcafee-cleaned-alert](Parsers/parserContent_s-mcafee-cleaned-alert.md)<br> ↳ [n-forwarded-cef-mcafee-epo](Parsers/parserContent_n-forwarded-cef-mcafee-epo.md)<br> ↳ [s-mcafee-deleted-alert](Parsers/parserContent_s-mcafee-deleted-alert.md)<br> ↳ [s-mcafee-epo-alert](Parsers/parserContent_s-mcafee-epo-alert.md)<br> ↳ [s-mcafee-clean-failed-alert](Parsers/parserContent_s-mcafee-clean-failed-alert.md)<br> ↳ [s-mcafee-epo-alert-2](Parsers/parserContent_s-mcafee-epo-alert-2.md)<br> ↳ [cef-mcafee-security-alert](Parsers/parserContent_cef-mcafee-security-alert.md)<br> ↳ [cef-mcafee-security-alert-1](Parsers/parserContent_cef-mcafee-security-alert-1.md)<br> ↳ [mcafee-epp-alert](Parsers/parserContent_mcafee-epp-alert.md)<br> ↳ [q-mcafee-epo-alert](Parsers/parserContent_q-mcafee-epo-alert.md)<br> ↳ [mcafee-vse-epo-alert](Parsers/parserContent_mcafee-vse-epo-alert.md)<br> ↳ [syslog-mcafee-epo-alert](Parsers/parserContent_syslog-mcafee-epo-alert.md)<br> ↳ [u-mcafee-epo-alert](Parsers/parserContent_u-mcafee-epo-alert.md)<br> ↳ [json-mcafee-epo-alert](Parsers/parserContent_json-mcafee-epo-alert.md)<br> ↳ [cef-mcafee-epo-alert-1](Parsers/parserContent_cef-mcafee-epo-alert-1.md)<br> ↳ [json-mcafee-epo-alert-1](Parsers/parserContent_json-mcafee-epo-alert-1.md)<br> ↳ [cef-mcafee-vse-alert](Parsers/parserContent_cef-mcafee-vse-alert.md)<br> ↳ [s-mcafee-security-alert](Parsers/parserContent_s-mcafee-security-alert.md)<br> ↳ [s-mcafee-security-alert-1](Parsers/parserContent_s-mcafee-security-alert-1.md)<br> ↳ [cef-mcafee-epo-alert-2](Parsers/parserContent_cef-mcafee-epo-alert-2.md)<br><br> usb-insert<br> ↳ [cef-mcafee-usb-insert](Parsers/parserContent_cef-mcafee-usb-insert.md)<br> ↳ [mcafee-dlp-rem-stor](Parsers/parserContent_mcafee-dlp-rem-stor.md)<br> ↳ [mcafee-dlp-pnp](Parsers/parserContent_mcafee-dlp-pnp.md)<br> ↳ [mcafee-dlp-pnp-2](Parsers/parserContent_mcafee-dlp-pnp-2.md)<br> ↳ [mcafee-dlp-rem-stor-2](Parsers/parserContent_mcafee-dlp-rem-stor-2.md)<br> ↳ [mcafee-dlp-mem-dev](Parsers/parserContent_mcafee-dlp-mem-dev.md)<br><br> usb-write<br> ↳ [mcafee-usb-write](Parsers/parserContent_mcafee-usb-write.md)<br> ↳ [s-mcafee-usb-activity](Parsers/parserContent_s-mcafee-usb-activity.md)<br> ↳ [syslog-mcafee-usb-activity](Parsers/parserContent_syslog-mcafee-usb-activity.md)<br> ↳ [cef-mcafee-usb-activity-1](Parsers/parserContent_cef-mcafee-usb-activity-1.md)<br> ↳ [n-forwarded-cef-mcafee-epo-usb](Parsers/parserContent_n-forwarded-cef-mcafee-epo-usb.md)<br> ↳ [cef-mcafee-usb-activity](Parsers/parserContent_cef-mcafee-usb-activity.md)<br> ↳ [mcafee-dlp-rem-stor](Parsers/parserContent_mcafee-dlp-rem-stor.md)<br> ↳ [mcafee-dlp-pnp](Parsers/parserContent_mcafee-dlp-pnp.md)<br> ↳ [mcafee-dlp-pnp-2](Parsers/parserContent_mcafee-dlp-pnp-2.md)<br> ↳ [mcafee-dlp-rem-stor-2](Parsers/parserContent_mcafee-dlp-rem-stor-2.md)<br> ↳ [mcafee-dlp-mem-dev](Parsers/parserContent_mcafee-dlp-mem-dev.md)<br> | T1052 - Exfiltration Over Physical Medium<br>T1066 - T1066<br>T1068 - Exploitation for Privilege Escalation<br>T1078 - Valid Accounts<br>T1133 - External Remote Services<br>T1188 - T1188<br>T1204 - User Execution<br> | [<ul><li>34 Rules</li></ul><ul><li>12 Models</li></ul>](Rules_Models/r_m_mcafee_mcafee_endpoint_security_Other.md) |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution                                                           | Persistence                                                                                                                                      | Privilege Escalation                                                                                                                                          | Defense Evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration                                                                           | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | -------------------------------------------------------------------------------------- | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Exploitation for Privilege Escalation](https://attack.mitre.org/techniques/T1068)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     | [Exfiltration Over Physical Medium](https://attack.mitre.org/techniques/T1052)<br><br> |        |