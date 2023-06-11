Summary:
Our e-commerce platform experienced a significant outage on September 5, 2021, from 2:00 PM to 6:00 PM (GMT), affecting the majority of our customers. During this time, users were unable to add items to their cart, make payments, or access the website. The outage was caused by a server crash, rendering the website inaccessible.

Timeline:

2:00 PM: Our monitoring alert system detected the issue.
2:05 PM: An engineer received a notification and began investigating.
2:10 PM: The engineer discovered that the server hosting the website had crashed.
2:15 PM: Attempting to resolve the issue, the engineer restarted the server without success.
2:20 PM: Recognizing a different cause than initially expected, the engineer escalated the issue to a senior engineer.
2:25 PM: The senior engineer identified an overloaded server due to a surge in traffic as the cause of the crash.
2:30 PM: Both engineers analyzed server logs and found evidence of attempted SQL injections and resource overloading.
2:45 PM: The platform development team was informed of a security vulnerability related to SQL injection.
3:00 PM: The platform development team conducted a code review, addressing overlooked vulnerabilities and initiating fixes.
4:00 PM: The issue was resolved, and the website and servers were operational again.

Root Cause and Resolution:
The outage resulted from a surge in traffic and attempted SQL injections, overwhelming the servers and causing the crash. The development team identified a security flaw in the code that enabled SQL injection. They deployed a security patch to eliminate the vulnerability, resolving the issue and restoring the platform.

Corrective and Preventative Measures:
To prevent future outages, we implemented the following measures:
1. Strengthened input validation functions, database connection functions, and error handling in the e-commerce platform.
2. Deployed a Web Application Firewall for protection against SQL injections, DDoS attacks, and other web-based threats.
3. Improved monitoring system to detect unusual traffic spikes and high resource usage, notifying engineers promptly.
4. Conducted a comprehensive review of the code, platform, and software components to identify weaknesses and vulnerabilities for patching, minimizing the risk of similar errors.

In conclusion, the outage was caused by a server crash resulting from a security flaw enabling attempted SQL injections and overwhelming the servers with increased traffic. We resolved the issue by deploying a patch and addressing the vulnerability. Additionally, we implemented measures such as a web application firewall and strengthened various functions to prevent similar outages in the future. Our team remains vigilant in monitoring the system to ensure optimal functionality.





