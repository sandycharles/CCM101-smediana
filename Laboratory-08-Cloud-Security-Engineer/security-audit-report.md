# Security Audit Report

## The Principle of Least Privilege (PoLP)
The Principle of Least Privilege means giving each user or program only the access it needs to do its job, and nothing more. It is important for cloud user accounts because if an account is hacked or misused by mistake, the damage is limited to what that account could access. For example, a user who only views reports should not be able to delete servers.

## Attack Surface
The attack surface of a virtual machine is the total number of places where an attacker could try to get in, such as open ports, running services, and user accounts. The more services and ports that are open, the more chances an attacker has to find a weakness. Keeping the attack surface small makes the server harder to compromise.

## Default Deny Policy
A Default Deny policy means all traffic is blocked unless it is specifically allowed. It is safer than blocking hackers one by one because it is impossible to know every attacker's address in advance, and new threats appear all the time. With default deny, anything that was forgotten or is unknown is still blocked.
