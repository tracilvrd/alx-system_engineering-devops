Issue Summary:
On 5th September 2021, from 2:00 PM to 6:00 PM (GMT), our e-commerce platform faced an outage, which impacted almost all of our customers. The users were unable to add any items to their cart, make payments or even access the website. The outage was caused by a server crash, which resulted in the website's inaccessibility.

Timeline:
- 2:00 PM: The issue was first detected by the monitoring alert system. 
- 2:05 PM: An engineer was notified about the issue and began investigating it.
- 2:10 PM: The engineer pieced together the puzzle and found out that the server hosting the website had crashed.
- 2:15 PM: The engineer attempted to fix the issue by restarting the server, but it didn't work.
- 2:20 PM: The engineer escalated the issue to the senior engineer as they found out that the cause was something different than expected.
- 2:25 PM: The senior engineer noticed the overloaded server caused by a surge in traffic, which resulted in the server crashing.
- 2:30 PM: Both engineers began analyzing server logs and identified several attempts for SQL injection as well as overloading of server resources that caused the crash.
- 2:45 PM: The platform development was notified about the issue as the cause was identified as a security vulnerability, which freed the SQL injection.
- 3:00 PM: The platform development team conducted a code review of the e-commerce platform and identified vulnerabilities that were overlooked. They commenced fixing it.
- 4:00 PM: The issue was resolved, and the website was back online, and the servers were operating normally.

Root cause and Resolution:
As mentioned, the root cause of the outage was caused by a surge in traffic and several attempted SQL injections. The servers were overloaded, and it caused the server to crash. The development team identified that there was a security flaw in the code that allowed the SQL injection. The team deployed a security patch that eliminated the vulnerability, and this allowed the team to fix the issue and get the platform back online.

Corrective and Preventative Measures:
To prevent a similar outage from happening in the future, here are some of the measures that were taken:
- Strengthening of the input validation functions, database connection functions, and error handling in the e-commerce platform.
- Deploying a Web Application Firewall to protect against SQL injections, DDoS, and other web-based attacks.
- Improved monitoring system implementation that can notify the engineers in case of any unusual traffic spikes or high resource usage.
- Conducting a thorough review of the code, platform as well as the software and its components to identify any weaknesses and vulnerabilities for patches to avoid similar errors in the future. 

In summary, the server crash and eventual outage were caused by a security flaw in the website's code that resulted in an attempted SQL injection and an overloaded server, crashing with surge traffic. The issue was resolved by deploying a patch to the vulnerability and fixing the cause of the vulnerability. We have also taken several measures to avoid similar outages in the future by implementing a web application firewall as well as strengthening our input validation, database connection, and error handling functions. We will continue to monitor our system closely to ensure that everything is functioning correctly.
