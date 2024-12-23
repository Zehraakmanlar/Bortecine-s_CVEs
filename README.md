# Open Redirect

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

## Exploting:
[![Alt text](https://img.youtube.com/vi/IMlZVgbwsLM/0.jpg)](https://www.youtube.com/watch?v=IMlZVgbwsLM) 
