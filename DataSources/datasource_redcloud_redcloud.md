Vendor: RedCloud
================
Product: RedCloud
-----------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   2   |   1    |     1      |      1      |    1    |

|                                 Use-Case                                  | Activity Types                            | Event Types/Parsers                                                                                                                                                                                                                                       | MITRE TTP                  | Content                                             |
|:-------------------------------------------------------------------------:| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- | --------------------------------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | <ul><li>Activity Time  and Type</li></ul> |  failed-physical-access<br> ↳ [redcloud-physical-badge-access](../Parsers/parserContent_redcloud-physical-badge-access.md)<br><br> physical-access<br> ↳ [redcloud-physical-badge-access](../Parsers/parserContent_redcloud-physical-badge-access.md)<br> | T1078 - Valid Accounts<br> | <ul><li>1 Rules</li></ul><ul><li>1 Models</li></ul> |
|        [Lateral Movement](../UseCases/usecase_lateral_movement.md)        | <ul><li>Badge Access</li></ul>            |  failed-physical-access<br> ↳ [redcloud-physical-badge-access](../Parsers/parserContent_redcloud-physical-badge-access.md)<br><br> physical-access<br> ↳ [redcloud-physical-badge-access](../Parsers/parserContent_redcloud-physical-badge-access.md)<br> | T1078 - Valid Accounts<br> | <ul><li>1 Rules</li></ul>                           |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     |              |        |