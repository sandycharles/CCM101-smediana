# Mission Reflection

## 1. How does a host-based firewall protect a server even if the physical network perimeter is breached?
A host-based firewall runs on the server itself, so it acts as the last line of defense. Even if an attacker gets past the network perimeter or is already inside the network, the firewall still checks every connection and blocks anything that is not explicitly allowed.

## 2. Why is managing open network ports critical to reducing a server's attack surface?
Every open port is a running service that attackers can probe for weaknesses, outdated software, or weak passwords. By keeping only the ports we need open, like SSH and 8080, we remove many possible entry points and make the server harder to attack.

## 3. Why is it dangerous to leave a database port (like 3306 for MySQL) open to the public internet?
If port 3306 is public, anyone in the world can try to guess passwords or exploit bugs in the database software. A successful attack could expose or delete sensitive data such as customer records. Databases should only be reachable by the application server through a private network.

## 4. How did completing this mission change your perspective on how easily a server can be compromised?
I learned that a server with no firewall is exposed from the moment it goes online, and attackers scan for open ports automatically. It also surprised me how quickly I could lock it down with just a few commands, which shows that good security does not have to be complicated.

## 5. How does your GitHub portfolio currently look with eight completed missions?
My GitHub portfolio now has eight organized laboratory folders, each with its own README, documentation, and screenshots. It shows my progress from basic cloud concepts to security, and it can serve as proof of my skills for future employers.
