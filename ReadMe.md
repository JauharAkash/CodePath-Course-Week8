# Project 8 - Pentesting Live Targets

Time spent: 5 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection
https://github.com/JauharAkash/codepathweek8/blob/master/SQL_injection.gif

Used the techniques of SQL injections learnt in the first few weeks of this course. Used ‘ in the URL to exploit and modify the URL.


Vulnerability #2: Session Hijacking
https://github.com/JauharAkash/codepathweek8/blob/master/Session_hijacking.gif

Changed the session id using the tools given. Also, applied tools from previous weeks.


## Green

Vulnerability #1: Enumeration
https://github.com/JauharAkash/codepathweek8/blob/master/Enumeration.gif

Logged in as “Admin” and saw the statement “log in was successful”. But when logged in as the username given in the instructions: “jmonroe99”. Saw that the statement “log in was successful” was bolded. 

Vulnerability #2: XSS
https://github.com/JauharAkash/codepathweek8/blob/master/XSS_attack.gif

Used the techniques of cross-site scripting. Left a malicious script under the feedback section. Gave me access to alter and attack the webpage (website).




## Red

Vulnerability #1: IDOR
https://github.com/JauharAkash/codepathweek8/blob/master/IDOR.gif

Changed the query parameter: ?id=__ several times. Enabled me to access pages that I didn’t have the permission too.


Vulnerability #2: CSRF
https://github.com/JauharAkash/codepathweek8/blob/master/CSRF.gif

Altered the user’s information on the webpage. Inspect tool helped to see the altered changes. Created the a “new” HTML file which made the changed onto the old HTML file without using the CSRF token.



