# web-security-week-8

# Project 8 - Pentesting Live Targets

Time spent: **4** hours spent in total

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

Vulnerability #1: Session Hijacking/Fixation: Changing the target's session ID to the attacker's logged in session ID allows the target access to admin features without first logging in.
<img src ="https://github.com/noodlesny/web-security-week-8/blob/master/myGifs/Week%208-Exploit%20Blue%20Really%20Really%20Real.gif" >

Vulnerability #2: SQL Injection (SQLi): Using SQLi adding a sleep query allows a delay in the page loading.
<img src= "https://github.com/noodlesny/web-security-week-8/blob/master/myGifs/Week%208-Exploit%20Blue%20Real%202.gif" >


## Green

Vulnerability #1: Cross Site Scripting: Input in the comment box isn't sanitized, so adding a script to a comment allows for an alert box to pop up when a user logs in and clicks on feedback. 
<img src= "https://github.com/noodlesny/web-security-week-8/blob/master/myGifs/Week%208-Exploit%20Green%20Real%201.gif?raw=true" >

Vulnerability #2: User Enumeration: There is different styling (normal and bold font) for log in errors of valid and invalid usernames.
<img src= "https://github.com/noodlesny/web-security-week-8/blob/master/myGifs/Week%208-Exploit%20Green%20Real%202.gif?raw=true" >

## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR): The ID for each salesman is visible in the URL, by manipulating the numbers, you are able to access 2 salesmen, 1 that had been terminated and 1 that is not supposed to be public until a later date.
<img src= "https://github.com/noodlesny/web-security-week-8/blob/master/myGifs/Week%208-Exploit%20Red%20Real%201.gif?raw=true" >

Vulnerability #2: Cross-Site Request Forgery (CSRF): Changing the token on the page should render it invalid, but it still works after it is changed.


## Notes
