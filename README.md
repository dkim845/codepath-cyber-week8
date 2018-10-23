# codepath-cyber-week8

# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

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

Vulnerability #1: SQL Injection (SQLi)

We performed a SQL Injection at the '/blue/public/salesperson.php?id=?' endpoint by replacing the parameter for 'id=?' with ' OR SLEEP(5)=0--' which caused the page to pause for 5 seconds, indicating a successful injection.

![](week8_blue1.gif)

Vulnerability #2: Session Hijacking/Fixation

In this exploit we used two different browsers to manipulate the session IDS. We took the PHPSESSIONID token of a user that was already logged in and set the different instance to the same token. The user could then bypass the login form and directly access the account that the session token belonged to.

![](week8_blue2.gif)


## Green

Vulnerability #1: __________________

Vulnerability #2: __________________


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
