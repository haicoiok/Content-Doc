Vendor: Specops
===============
Product: Specops Password Reset
-------------------------------
|                                 Use-Case                                  | Activity Types            | Event Types/Parsers                                                                                                                                                                                                                              | MITRE TTP                  | Content                   |
|:-------------------------------------------------------------------------:| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------- | ------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | - Activity Time  and Type |  account-password-reset<br> -- [specops-account-password-reset](../Parsers/parserContent_specops-account-password-reset.md)<br><br> account-unlocked<br> -- [specops-account-unlocked](../Parsers/parserContent_specops-account-unlocked.md)<br> | T1078 - Valid Accounts<br> |  - 1 Rules<br> - 1 Models |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilage escalation                                                | Defense evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     |              |        |