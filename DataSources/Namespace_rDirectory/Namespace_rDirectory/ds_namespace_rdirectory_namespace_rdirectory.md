Vendor: Namespace rDirectory
============================
Product: Namespace rDirectory
-----------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   9   |   6    |     4      |      7      |    7    |

|                Use-Case                | Activity Types                                                                                                                                    | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | MITRE TTP                                                                                                                                    | Content                                                                                                                    |
|:--------------------------------------:| ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| [Other](../../../UseCases/uc_other.md) | <ul><li>Account Creation and Management</li><li>Activity Time  and Type</li><li>Asset Logon and Access</li><li>Critical System Activity</li></ul> |  account-creation<br> ↳ [rdirectory-account-created](Parsers/parserContent_rdirectory-account-created.md)<br><br> account-deleted<br> ↳ [rdirectory-account-deleted](Parsers/parserContent_rdirectory-account-deleted.md)<br><br> account-disabled<br> ↳ [rdirectory-account-disable](Parsers/parserContent_rdirectory-account-disable.md)<br><br> account-enabled<br> ↳ [rdirectory-account-enable](Parsers/parserContent_rdirectory-account-enable.md)<br><br> account-password-change<br> ↳ [rdirectory-password-change](Parsers/parserContent_rdirectory-password-change.md)<br><br> ds-access<br> ↳ [rdirectory-object-modification](Parsers/parserContent_rdirectory-object-modification.md)<br><br> member-added<br> ↳ [rdirectory-member-added](Parsers/parserContent_rdirectory-member-added.md)<br> | T1003 - OS Credential Dumping<br>T1068 - Exploitation for Privilege Escalation<br>T1078 - Valid Accounts<br>T1098 - Account Manipulation<br> | [<ul><li>9 Rules</li></ul><ul><li>6 Models</li></ul>](Rules_Models/r_m_namespace_rdirectory_namespace_rdirectory_Other.md) |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                                                                                                  | Privilege Escalation                                                                                                                                          | Defense Evasion                                                     | Credential Access                                                          | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Account Manipulation](https://attack.mitre.org/techniques/T1098)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Exploitation for Privilege Escalation](https://attack.mitre.org/techniques/T1068)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [OS Credential Dumping](https://attack.mitre.org/techniques/T1003)<br><br> |           |                  |            |                     |              |        |