# Open Redirect

# CVE-2024-51112
+ *Exploit Author:* Fatime Zehra AKMANLAR
+ *Vendor Homepage:* https://www.pnetlab.com/pages/main
+ *Software Link:* https://pnetlab.com/pages/releases
+ *Version:* 5.3.11
+ *Tested on:* Windows 10 Home
  
## Description:
+ An Open Redirect Vulnerability entails an attacker manipulating the user and redirecting them from one site to another site – which may be malicious.
I add any link between the parameters “box=&link” and then when I log in, it forwards to the link I added.

## References: 
+ https://portswigger.net/kb/issues/00500100_open-redirection-reflected

## Proof of concept:
+ Install PNETLab on VMware and access the login page using the assigned interface IP.
+ Once accessed, add another URL to the link parameter in the current URL and press Enter. For example, https://google.com.
+ Enter your login credentials in the respective fields.
+ Press Enter.
+ You will be redirected to google.com.

## Exploiting:
[![Alt text](https://img.youtube.com/vi/IMlZVgbwsLM/0.jpg)](https://www.youtube.com/watch?v=IMlZVgbwsLM) 

*************************************************************************************************************

# Reflected_XSS

# CVE-2024-51111
+ *Exploit Author:* Fatime Zehra AKMANLAR
+ *Vendor Homepage:* https://www.pnetlab.com/pages/main
+ *Software Link:* https://pnetlab.com/pages/releases
+ *Version:* 5.3.11
+ *Tested on:* Windows 10 Home
  
## Description:
+In XSS (Cross-Site Scripting) attacks, manipulating the 'success' parameter can allow attackers to execute malicious code via application error messages or other user interactions.

## References: 
+ https://portswigger.net/web-security/cross-site-scripting

## Proof of concept:
+ Install PNETLab on VMware and access the interface using the assigned interface IP.
+ Register on the interface. 
+ After registration, it will redirect you to the login page(https://authen.pnetlab.com/login?success=Thank%20you%20for%20contributing%20to%20building%20the%20PNETLab%20community.%20%0A%20%20%20%20%20%20%20%20Please%20check%20your%20email%20%3Cb%3Edeneme123@gmail.com%3C/b%3E%20to%20activate%20your%20account.%20If%20you%20do%20not%20receive%20the%20email%20please%20check%20the%20junk%20email%20or%20contact%20us%20at%20the%20website%20www.PNETLab.com)  ,where you need to add the <script>alert("bortecine")</script> script to the success parameter in the relevant URL.
+ XSS will be loaded.
+ Alerts will pop up.

## Exploiting:
[![Alt text](https://img.youtube.com/vi/2WTILpEeplo/0.jpg)](https://www.youtube.com/watch?v=2WTILpEeplo)
