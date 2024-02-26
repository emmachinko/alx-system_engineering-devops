0. Simple web stack

* What is a server
Servers are physical machines (as hardwares), virtual machines or softwares (computer programs) that serve or provide functionality to other programs or devices called “clients”. The term server comes from queuing theory used in Kendall’s notation, where servers serve or process the clients requirements in the same way as a telephone operator, a cooker or a production machine process incoming orders, having in mind its capacity and service process time

A computer can function as a server, and a server can be a computer, both of them being built up with hardware and software. However, the main difference between these two is the capacity and computer power servers have. In other words, servers are computers on steroids with faster processing capacity. They are usually stored in data centers racks (stacks of servers piled one on top of each other).

* What is the role of the domain name
Domain names serve to identify Internet resources, such as computers, networks, and services, with a text-based label that is easier to memorize than the numerical addresses used in the Internet protocols.

* What type of DNS record www is in www.foobar.com
DNS record of www belongs to a subdomain of the www.foobar.com

* What is the role of the web server?
The primary role of a web server is to store, process, and deliver requested information or webpages to end users.

* What is the role of the application server?
The main function of a Web server is to store the files of a site and broadcast them over the Internet so that they can be visited by users. Basically, a web server is a large computer that stores and transmits data via the network system called the Internet. When a user enters an Internet page, his browser communicates with the server sending and receiving data that determines what he sees on the screen. Therefore, we say that Web servers are to store and transmit data from a site as requested by a visitor’s browser.

* What is the role of the database?
The primary purpose of a database is to store, retrieve, and update information. A database can be used to store data related to any aspect of business operations. Databases can be very large, containing millions of records, or very small, containing just a few records or even a single record.

* What is the server using to communicate with the computer of the user requesting the website?
The server is using the HTTP (Hypertext Transfer Protocol), which enables the transfer of resource and data, such as HTML documents between the server and the client. In this data exchange the request is initiated by the client, which is done normally by web browser (it can also be done by an operating sistem or application) are called request and the server answers are called responses. Between the client and server data exchange we can find numerous entintes, collectively called proxies, performing different operations such as gateways or caches.

* issues are with this infrastructure:  
 • SPOF
A single point of failure (SPOF) is a part of a system that, if it fails, will stop the entire system from working. SPOFs are undesirable in any system with a goal of high availability or reliability, be it a business practice, software application, or other industrial system.
To eliminate single points of failure, first identify potential risk posed by conducting a single point of failure risk assessment across three main areas: hardware, software/providers/services, and people. Create a single point of failure analysis checklist detailing the general areas for assessment.

 • Downtime when maintenance needed (like deploying new code web server needs to be restarted)
downtime in web server is When a website or web service is not available online or doesn't function well enough for end users to complete a task.
whenever some structure or node in the system needs to be repaired, the whole system has to be shut down, while the maintenance is done. Then, client requests cannot be attended during this period of time.

 • Cannot scale if too much incoming traffic
Overload of traffic can be a risk to the server capacity. This, because there is no possibility to scale the service with additional servers as backup. Leading to a possible breakdown of the web page and client requests, as traffic surpasess servers capacity.
