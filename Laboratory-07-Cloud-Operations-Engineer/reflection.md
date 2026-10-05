# Mission 7 Reflection

## 1. Why is it important to check the host server's resources even if your containers are running perfectly?

Containers share the host's CPU, RAM, and disk, so a container can look healthy while the host is quietly running out of resources. If the host's memory or disk fills up, every container on it can slow down, crash, or fail to write data. In this lab, my host had 1.9 GiB of RAM and 19 GB of disk, so checking them gave me a baseline to compare against later.

## 2. If a user complains that they cannot log into a web application, how would the docker logs command help you solve the problem?

I would run docker logs on the application's container and look at the entries around the time the user tried to log in. Status codes such as 401 or 403 suggest wrong credentials or blocked access, while a 500 points to a server-side failure. The error messages in the logs would show the exact cause, so I can fix the real problem instead of guessing.

## 3. What is the difference between monitoring logs and monitoring metrics?

Logs are records of individual events, such as my 404 request to /hidden-admin-page, and they tell me what happened and when. Metrics are numbers measured over time, such as the container's 0.00% CPU and 2.738MiB memory in docker stats, and they tell me how the system is performing. Logs help explain a specific problem, while metrics help me spot trends and overload.

## 4. How do large enterprise companies monitor thousands of containers at the same time?

Large companies cannot check containers one by one, so they use monitoring tools. Prometheus automatically collects and stores metrics from many containers, and Grafana turns that data into dashboards and sends alerts when a value crosses a limit. This gives the operations team one central view of thousands of containers.

## 5. How has your ability to troubleshoot Linux environments improved?

Before this lab, I only knew basic commands. Now I can check memory with free -h, check disk space with df -h, read application logs with docker logs, and watch live usage with docker stats. I also learned to rely on evidence from logs and metrics instead of guessing. When the q key did not exit top, I learned to use Ctrl+C or another terminal tab instead.
