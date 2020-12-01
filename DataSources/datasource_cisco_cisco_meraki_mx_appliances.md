Vendor: Cisco
=============
Product: Cisco Meraki MX appliances
-----------------------------------
|                                 Use-Case                                  | Activity Types                                                                                                                                                                                                                          | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | MITRE TTP                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Content                    |
|:-------------------------------------------------------------------------:| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | - Activity Time  and Type<br>- Application Activity<br>- Asset Logon and Access<br>- Credential Switch Activity<br>- Email Activity<br>- Network zones and Location Access<br>- Privileged Activity<br>- VPN Activity<br>- Web Activity |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1003 - OS Credential Dumping<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1078 - Valid Accounts<br>T1098 - Account Manipulation<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>T1110 - Brute Force<br>T1133 - External Remote Services<br>T1558.003 - Steal or Forge Kerberos Tickets: Kerberoasting<br>                                                                                                                                                                                 |  - 32 Rules<br> - 8 Models |
|       [Data Exfiltration](../UseCases/usecase_data_exfiltration.md)       | - Application Activity<br>- Data Loss Prevention<br>- Email Activity<br>- Web Activity                                                                                                                                                  |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1030 - Data Transfer Size Limits<br>T1048.003 - Exfiltration Over Alternative Protocol: Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol<br>T1052 - Exfiltration Over Physical Medium<br>T1052.001 - Exfiltration Over Physical Medium: Exfiltration over USB<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1078 - Valid Accounts<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>T1566 - Phishing<br>T1567.002 - Exfiltration Over Web Service: Exfiltration to Cloud Storage<br> |  - 11 Rules<br>            |
|          [Internal Fraud](../UseCases/usecase_internal_fraud.md)          | - Application Activity<br>- Web Activity                                                                                                                                                                                                |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1071.001 - Application Layer Protocol: Web Protocols<br>T1078 - Valid Accounts<br>                                                                                                                                                                                                                                                                                                                                                                                                                                                    |  - 4 Rules<br> - 2 Models  |
|        [Lateral Movement](../UseCases/usecase_lateral_movement.md)        | - Asset Logon and Access<br>- Network<br>- Network Alert<br>- Network zones and Location Access<br>- Security Alert<br>- Web Activity                                                                                                   |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1027.005 - Obfuscated Files or Information: Indicator Removal from Tools<br>T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1078 - Valid Accounts<br>T1090.002 - Proxy: External Proxy<br>T1133 - External Remote Services<br>T1571 - Non-Standard Port<br>                                                                                                                                                                                                                           |  - 36 Rules<br> - 7 Models |
|       [Malware Detection](../UseCases/usecase_malware_detection.md)       | - Asset Logon and Access<br>- Email Activity<br>- Endpoint Activity<br>- Network<br>- Process Activity<br>- Web Activity                                                                                                                |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1078 - Valid Accounts<br>T1090.002 - Proxy: External Proxy<br>T1090.003 - Proxy: Multi-hop Proxy<br>T1102 - Web Service<br>T1204 - User Execution<br>T1496 - Resource Hijacking<br>T1550.002 - Use Alternate Authentication Material: Pass the Hash<br>T1566 - Phishing<br>T1568 - Dynamic Resolution<br>T1568.002 - Dynamic Resolution: Domain Generation Algorithms<br>T1571 - Non-Standard Port<br>                                 |  - 64 Rules<br> - 5 Models |
|                [Phishing](../UseCases/usecase_phishing.md)                | - Email Activity<br>- Network<br>- Web Activity                                                                                                                                                                                         |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1566 - Phishing<br>T1566.002 - Phishing: Spearphishing Link<br>T1568 - Dynamic Resolution<br>                                                                                                                                                                                                                                                                                                                                          |  - 10 Rules<br>            |
|     [Privileged Activity](../UseCases/usecase_privileged_activity.md)     | - Application Activity<br>- Credential Switch Activity<br>- Privileged Activity                                                                                                                                                         |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1003 - OS Credential Dumping<br>T1078 - Valid Accounts<br>T1098 - Account Manipulation<br>                                                                                                                                                                                                                                                                                                                                                                                                                                            |  - 6 Rules<br> - 1 Models  |
|    [Ransomware Detection](../UseCases/usecase_ransomware_detection.md)    | - Asset Logon and Access<br>- Email Activity<br>- Endpoint Activity<br>- Network<br>- Process Activity<br>- Web Activity                                                                                                                |  network-alert<br> -- [cef-meraki-network-alert](../Parsers/parserContent_cef-meraki-network-alert.md)<br> -- [meraki-network-alert](../Parsers/parserContent_meraki-network-alert.md)<br><br> network-connection-failed<br> -- [meraki-network-connection](../Parsers/parserContent_meraki-network-connection.md)<br><br> network-connection-successful<br> -- [meraki-ip-flow-start](../Parsers/parserContent_meraki-ip-flow-start.md)<br> -- [meraki-network-connection-1](../Parsers/parserContent_meraki-network-connection-1.md)<br><br> vpn-login<br> -- [cisco-meraki-vpn-start](../Parsers/parserContent_cisco-meraki-vpn-start.md)<br><br> vpn-logout<br> -- [cisco-meraki-vpn-stop](../Parsers/parserContent_cisco-meraki-vpn-stop.md)<br><br> web-activity-allowed<br> -- [cisco-meraki-web-activity](../Parsers/parserContent_cisco-meraki-web-activity.md)<br><br> web-activity-denied<br> -- [meraki-web-activity-denied](../Parsers/parserContent_meraki-web-activity-denied.md)<br> | T1071 - Application Layer Protocol<br>T1071.001 - Application Layer Protocol: Web Protocols<br>T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br>T1102 - Web Service<br>T1204 - User Execution<br>T1496 - Resource Hijacking<br>T1550.002 - Use Alternate Authentication Material: Pass the Hash<br>T1566 - Phishing<br>T1568 - Dynamic Resolution<br>T1568.002 - Dynamic Resolution: Domain Generation Algorithms<br>                                                                                                   |  - 47 Rules<br> - 4 Models |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                                                                                                                                                                     | Execution                                                           | Persistence                                                                                                                                                                                                                                                                                                                                 | Privilage escalation                                                | Defense evasion                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Credential Access                                                                                                                                                                                                                                                                                                                     | Discovery | Lateral Movement                                                                           | Collection | Command and Control                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Exfiltration                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Impact                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | ------------------------------------------------------------------------------------------ | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------- |
| [Phishing: Spearphishing Link](https://attack.mitre.org/techniques/T1566/002)<br><br>[External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Phishing](https://attack.mitre.org/techniques/T1566)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Account Manipulation](https://attack.mitre.org/techniques/T1098)<br><br>[Account Manipulation: Exchange Email Delegate Permissions](https://attack.mitre.org/techniques/T1098/002)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Obfuscated Files or Information: Indicator Removal from Tools](https://attack.mitre.org/techniques/T1027/005)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Use Alternate Authentication Material](https://attack.mitre.org/techniques/T1550)<br><br>[Use Alternate Authentication Material: Pass the Hash](https://attack.mitre.org/techniques/T1550/002)<br><br>[Obfuscated Files or Information](https://attack.mitre.org/techniques/T1027)<br><br> | [OS Credential Dumping](https://attack.mitre.org/techniques/T1003)<br><br>[Brute Force](https://attack.mitre.org/techniques/T1110)<br><br>[Steal or Forge Kerberos Tickets](https://attack.mitre.org/techniques/T1558)<br><br>[Steal or Forge Kerberos Tickets: Kerberoasting](https://attack.mitre.org/techniques/T1558/003)<br><br> |           | [Use Alternate Authentication Material](https://attack.mitre.org/techniques/T1550)<br><br> |            | [Web Service](https://attack.mitre.org/techniques/T1102)<br><br>[Non-Standard Port](https://attack.mitre.org/techniques/T1571)<br><br>[Application Layer Protocol: Web Protocols](https://attack.mitre.org/techniques/T1071/001)<br><br>[Dynamic Resolution](https://attack.mitre.org/techniques/T1568)<br><br>[Dynamic Resolution: Domain Generation Algorithms](https://attack.mitre.org/techniques/T1568/002)<br><br>[Proxy: Multi-hop Proxy](https://attack.mitre.org/techniques/T1090/003)<br><br>[Proxy: External Proxy](https://attack.mitre.org/techniques/T1090/002)<br><br>[Application Layer Protocol](https://attack.mitre.org/techniques/T1071)<br><br>[Proxy](https://attack.mitre.org/techniques/T1090)<br><br> | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br>[Exfiltration Over Alternative Protocol: Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol](https://attack.mitre.org/techniques/T1048/003)<br><br>[Exfiltration Over Physical Medium: Exfiltration over USB](https://attack.mitre.org/techniques/T1052/001)<br><br>[Data Transfer Size Limits](https://attack.mitre.org/techniques/T1030)<br><br>[Exfiltration Over Physical Medium](https://attack.mitre.org/techniques/T1052)<br><br>[Exfiltration Over Web Service: Exfiltration to Cloud Storage](https://attack.mitre.org/techniques/T1567/002)<br><br>[Exfiltration Over Web Service](https://attack.mitre.org/techniques/T1567)<br><br> | [Resource Hijacking](https://attack.mitre.org/techniques/T1496)<br><br> |