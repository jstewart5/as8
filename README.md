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
- It is possible to escape the salesperson ID query and inject your own query.
![Alt Text](https://i.imgur.com/SYM76Mq.gif)

Vulnerability #2: __________________


## Green

Vulnerability #1: Username Enumeration
- An error message is retrieved when the wrong password is given. The message is only bold if the username is valid. This indicates that there are at least two different errors that can be retrieved. An intruder could use this information to check for valid usernames.
![Alt Text](https://i.imgur.com/noJvDwY.gif)

Vulnerability #2: Cross-Site Scripting (XSS)
- There is an unsanitized web form on the Contact Us page.
![Alt Text](https://i.imgur.com/SAATgKx.gif)

## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
