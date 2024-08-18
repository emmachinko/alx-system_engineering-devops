Incident report/postmortem August 16, 2024

Issue summary:

On August 16, 2024, from 9:00 AM to 2:00 PM GMT+2, users were unable to access our company's web application. The service  outage prevented all users attempting to log into the application during this time period, resulting in a 100% service outage. Users were experiencing an error message or service timeout when attempting to access the server.

Root Causes:

Our team identified the root cause of the issue as a configuration error in the load balancer. The load balancer had reached its connection limit, causing it to reject new connections to the web servers. And those already connected are facing system timeout due to software bugs.

Timeline:

- 9:00 AM GMT+2: The issue was detected through monitoring alerts of a high number of requests to the load balancer.

- 9:20 AM GMT+2: Our team began investigating the issue, assuming it was a database or application server issue.

- 10:00 AM GMT+2: After investigating the database and application server, it was discovered that the load balancer was the root cause.

- 10:20 AM GMT+2: The load balancer was restarted in an attempt to fix the issue.

- 10:50 AM GMT+2: The issue persisted after the restart, and our team escalated the incident to the network infrastructure team.

- 11:30 AM GMT+2: The network infrastructure team identified the configuration error in the load balancer and the bugs causing system timeout. They worked and resolved the issue.

- 2:00 PM GMT+2: The web server was fully restored and accessible to all users.

Misleading Investigation/Debugging Paths:

At first, our team assumed the issue was with the database or application servers. This assumption led to a delay in identifying the root cause thereby  escalating the incident to the appropriate team for proper investigation.

Escalation:

After the load balancer was restarted, as the problem persist, the incident was escalated to the network infrastructure team to do their part in indentifying the problem.

Resolution:

The network infrastructure team identified and corrected the configuration error in the load balancer, and with the help of bug tracker, the bug causing service timeout was detected and fixed. All this moves helped to restored full service to the web server.

Corrective and Preventative Measures:

To prevent similar outages from occurring in the future, our team has implemented the following measures:

- Increase monitoring of the load balancer to detect connection limit issues

- Review load balancer configurations to ensure they are optimized for our current traffic load

- Update incident response procedures to escalate issues to the appropriate team faster

- Conduct training sessions for team members on identifying and troubleshooting load balancer issues

TASK:

- Review and optimize load balancer configurations

- Increase monitoring of the load balancer

- Alerting mechanisms to provide timely notifications of service degradations.

- Conduct training sessions for team members

