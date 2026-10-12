# Mission Reflection

## 1. Why is automation critical when managing hundreds of cloud servers?
Typing commands one by one on hundreds of servers is too slow and easy to get wrong. Automation lets a single script do the same task on every server in the same way, every time. It also removes the need for someone to remember routine jobs like backups, which is exactly what failed for the client in this mission.

## 2. What are the potential dangers of automation?
The same speed that makes automation useful also makes mistakes spread quickly. A destructive typo, such as deleting the wrong folder, would run on all 1,000 servers at once and could cause huge data loss before anyone notices. To reduce this risk, scripts should be tested on one machine first, rolled out in small groups, and protected by backups.

## 3. How did writing a Bash script differ from creating a Docker Compose YAML file?
A Bash script is a list of steps that the computer follows in order, so I had to think about how to do each task. A Docker Compose YAML file describes the result I want, and Docker figures out the steps. Bash felt more hands-on and flexible, while Compose felt cleaner and easier to read.

## 4. How has my understanding of Cloud Computing transformed this semester?
In Laboratory 1, cloud computing felt like an abstract idea about renting servers over the internet. By Laboratory 9, I understood it as a set of skills: building infrastructure, deploying containers, monitoring, securing, and automating. I now see the cloud as something I can actually operate, not just define.

## 5. Which role did I enjoy the most and why?
I enjoyed the Cloud Automation Engineer role the most because I could see the result immediately. One script and one cron line replaced a manual task completely. It showed me how a small piece of code can prevent a real problem like lost customer files.
