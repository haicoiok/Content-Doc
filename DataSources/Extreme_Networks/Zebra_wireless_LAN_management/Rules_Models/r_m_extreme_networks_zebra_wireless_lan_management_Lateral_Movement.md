Vendor: Extreme Networks
========================
### Product: [Zebra wireless LAN management](../ds_extreme_networks_zebra_wireless_lan_management.md)
### Use-Case: [Lateral Movement](../../../../UseCases/uc_lateral_movement.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   2   |   1    |     3      |      1      |    1    |

| Event Type   | Rules                                                                                                                                                                                                                                                                                                                             | Models |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| failed-logon | <b>T1550.003 - Use Alternate Authentication Material: Pass the Ticket</b><b>T1550.004 - Use Alternate Authentication Material: Web Session Cookie</b><br> ↳ <b>KL-TfG</b>: Rare Kerberos ticket failure code<br><br><b>T1110 - Brute Force</b><br> ↳ <b>FL-MULTI-DEST-M</b>: Failed logins to multiple destinations from host (M) |        |