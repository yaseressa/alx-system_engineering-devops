Issue Summary:
Duration: June 20, 2023, 10:00 AM - June 21, 2023, 2:00 PM (PST)
Impact: The online shopping service experienced a complete outage for approximately 28 hours. During this time, users were unable to access the website, browse products, make purchases, or interact with their accounts. The outage affected 100% of the users, resulting in significant revenue loss and a negative impact on customer satisfaction.


Timeline:
June 20, 2023, 10:00 AM: The issue was detected when the monitoring system triggered an alert for high server response times.
Investigation began immediately, with the assumption that the database server was the root cause due to its critical role in serving the web application.
Multiple engineers were involved in analysing the database logs, network connectivity, and server performance metrics to identify the issue.
Misleading paths: Initially, it was suspected that a sudden spike in database connections or a network issue caused the outage. However, after thorough analysis, these assumptions proved to be incorrect.
The incident was escalated to the database operations team and senior management due to the severity of the outage and the inability to identify the root cause promptly.
The incident was resolved on June 21, 2023, 2:00 PM, after a comprehensive investigation and resolution process.
Root Cause and Resolution:
Root Cause: The root cause of the outage was a misconfigured caching layer between the web application and the database server. The cache was not properly configured to handle sudden increases in traffic and failed to invalidate outdated entries effectively.


Resolution: The issue was fixed by implementing the following steps:
Identified and corrected the misconfiguration in the caching layer to ensure proper handling of cache invalidation.
Conducted thorough testing and validation to verify the stability and performance of the web stack.
Implemented additional monitoring and alerting mechanisms to proactively identify any future cache-related issues.
Corrective and Preventative Measures:
To prevent similar incidents in the future, the following measures will be implemented:
Perform regular audits of system configurations and dependencies to identify potential misconfigurations and optimise performance.
Enhance monitoring and alerting systems to provide early detection of issues and minimise downtime.
Implement automated testing and validation processes to verify the correct functionality of critical components before deployment.
Develop and follow a comprehensive incident response plan to ensure efficient escalation and communication during future incidents.
Conduct post-incident reviews to identify further areas of improvement and share lessons learned with the engineering team.
Tasks to Address the Issue:
Review and update the caching layer configuration to handle variable traffic patterns and improve cache invalidation mechanisms.
Enhance monitoring system to provide real-time visibility into cache utilisation, response times, and error rates.
Implement automated testing to simulate and validate high load scenarios to ensure the stability of the web stack.
Document and distribute an incident response plan, including clear escalation paths and communication channels.
Conduct training sessions for the engineering team on incident management best practices and techniques.




In conclusion, the web stack outage was caused by a misconfigured caching layer, resulting in a complete service outage for 28 hours. The issue was resolved by fixing the misconfiguration and implementing additional measures to improve monitoring and caching mechanisms. Moving forward, the team will focus on implementing corrective and preventative measures to enhance system stability, responsiveness, and resilience to prevent similar incidents from occurring in the future.


