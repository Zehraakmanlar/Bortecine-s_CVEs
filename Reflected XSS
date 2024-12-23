# Reflected_XSS

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

## Exploting:
[![Alt text](https://img.youtube.com/vi/2WTILpEeplo/0.jpg)](https://www.youtube.com/watch?v=2WTILpEeplo)
