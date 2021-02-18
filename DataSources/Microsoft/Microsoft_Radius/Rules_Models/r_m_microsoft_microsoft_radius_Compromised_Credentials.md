Vendor: Microsoft
=================
### Product: [Microsoft Radius](../ds_microsoft_microsoft_radius.md)
### Use-Case: [Compromised Credentials](../../../../UseCases/uc_compromised_credentials.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   4   |   1    |     2      |      1      |    1    |

| Event Type | Rules                                                                                                                                                                                                                                                                                                               | Models                                  |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| nac-logon  | <b>T1021 - Remote Services</b><br> ↳ <b>NAC-GAt-A</b>: Abnormal authentication type for peer group<br> ↳ <b>NAC-UAt-F</b>: First authentication type for user<br> ↳ <b>NAC-UAt-A</b>: Abnormal authentication type for user<br><br><b>T1078 - Valid Accounts</b><br> ↳ <b>AE-UA-F</b>: First activity type for user |  • <b>AE-UA</b>: All activity for users |