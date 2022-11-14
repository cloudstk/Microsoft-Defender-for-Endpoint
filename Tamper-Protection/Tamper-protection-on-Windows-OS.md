

How to enable tamper protection on unmanaged PCs
==
When bad actors gain access to a system they often want to disable Microsoft Defender Antivirus, that way their malware 
and their suspicious activity are successful. There’s a feature available in Windows OS called tamper protection that 
prevents a bad actor or malicious application from disabling the Microsoft Defender Antivirus setting, including real-time 
protection and cloud-delivered protection.

Microsoft Defender for Endpoint will turn on tamper protection by default for all enterprise customers. If you are using a 
personal system that is not managed by an organization’s security team, you can manage tamper protection using the following steps.

Steps:
--
1. In the search box on the taskbar, type **Windows Security** and then select **Windows Security**. 

 ![Image](/Tamper-Protection/media/Windows10-Tamper-protection-01.jpg "icon") 
 
 2. In Windows Security, select **Virus & threat protection** and then under **Virus & threat protection settings**, select **Manage settings**.
 
  ![Image](/Tamper-Protection/media/Windows10-Tamper-protection-03.jpg "icon") 
 
 3. Change the **Tamper Protection** setting to **On**.

  ![Image](/Tamper-Protection/media/Windows10-Tamper-protection-04.jpg "icon") 

---
Use PowerShell to check Tamper Protection
--
1.	Open the **PowerShell application**.
2.	Enter the **Get-MPComputerStatus** PowerShell cmdlet.
3.	In the list of results, look for **IsTamperProtection**. If the value is **true**, then Tamper Protection is enabled.



Useful Links
--
[Protect security settings with tamper protection](https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/prevent-changes-to-security-settings-with-tamper-protection?view=o365-worldwide)
