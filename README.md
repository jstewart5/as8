# Project 8 - Pentesting Live Targets

Time spent: **7** hours spent in total

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
- The salesperson ID query is unsanitized here. The other sites just redirect to the territories page.

![Alt Text](https://i.imgur.com/SYM76Mq.gif)

Vulnerability #2: Session Hijacking/Fixation
- It is possible to bypass the login page if you change your session id to that of an already logged-in user.

![Alt Text](https://i.imgur.com/5vRncKu.gif)


## Green

Vulnerability #1: Username Enumeration
- An error message is retrieved when the wrong password is given. The message is only bold if the username is valid. This indicates that two errors are retrieved here. An intruder could use this information to check the site for valid usernames.

![Alt Text](https://i.imgur.com/noJvDwY.gif)

Vulnerability #2: Cross-Site Scripting (XSS)
- There is an unsanitized web form on the Contact Us page.

![Alt Text](https://i.imgur.com/SAATgKx.gif)

## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)
- By changing the salesperson ID, you can access pages that can't be found on the territories page.

![Alt Text](https://i.imgur.com/sSkI2PN.gif)

Vulnerability #2: Cross-Site Request Forgery (CSRF)
- The site fails to check the CSRF token. Any value can be used as a token to edit salesperson data.

![Alt Text](https://i.imgur.com/FzThLZz.gif)


## Notes

I wasn't able to retrieve anything from the SQLi vulnerability, only confirm its existence
