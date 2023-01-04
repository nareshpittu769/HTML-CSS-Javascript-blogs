# Server and how it works on different domains.

## "What is the server?"

The server is a program or a device which provides the functionalities or services to the other computers which are known as clients.

Here the client requests the data the server will serve the data based on the client's information.

Multiple clients will interact with the server at a time.

This is called the Client-Server model.

## "How does the Client interact with the server ?"

Here server sends the data and stores the data correctly, but how the client will interact with the server it is problem right?  
We have a solution for that, here we use "DNS" which is called **DOMAIN NAME SPACE**.  
So every website has the domain name by the help of this we are directed to the website that we are looking for.  
It looks like this "[www.domainname.com](http://www.domainname.com)". The domain name would be anything like "[google.com](http://google.com)" or "gmail.com" anything.

But internally the **DNS resolver** will convert the domain name into the ServerIP address. After that, the server will receive the request and it will produce the output to the client.

This process is done through the "internet".

## "Types of servers"

There are multiple types of servers they are:

* Web Server
    
* Application Server
    
* Database Server
    
* Game Server
    
* Mail Server
    
* Proxy Server
    
* Cloud Server
    

All the server provides the same functionality but different purposes use different servers.

**Web Server**  
The web server provides lots of data about the components of the website. The web server is always connected to the internet because if the host wants to change the data he can directly change the content.

The static site is known as we are storing the data in our local storage. So if any modifications are done to website content it is not reflected on the website. We have to explicitly save the content and we have to reload the site. That's why we are calling it "Static".

The website is "dynamic" because we don't need to reload the page every time any modifications are done on the website the site state is changed then the server will automatically update the content on the website. That's why we are calling it "Dynamic".

Here the website work based on the "HTTP" server. The HTTP server that understands the URLs and HTTP(Hypertext transfer protocol) or HTTPS(Hyper text transfer protocol secure). The HTTPS did not allow any third-party users it is secure.

Whenever a client requires a file that is hosted on a web server, the client requests the server by using HTTP. After the request reaches the web server the server will process it, it will find the correct data and respond to the client browser.  
**Types of Web servers**

1. Apache: It is a free and open-source web server which uses the HTTP server to access the data from the website through the internet.
    
2. Nginx: It is free and open source which uses the HTTP server to access the data from a website. It is better than the Apache.
    

3\. Microsoft IIS: To exchange information between the client and server.

**Application Server**  
The Application server provides the access to the web apps. Here we can directly access the data of a particular web app without install to our system. The Application server provides access to clients so they can easily interact with web apps.[  
](https://res.cloudinary.com/practicaldev/image/fetch/s--jr3SVuE0--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6ypzavrye46c6il66m0x.png)**Database Server**  
The Database server stores the data about the organization. Here we can store multiple data according to our requirements. We can use multiple servers to store multiple pieces of information.

**Game Server**  
The Game Server is the server that provides the data about the client while playing the game. The client wants data about his health, energy, guns etc. All the information is provided by the Game server.

**Mail Server**  
The Mail server provides the data about the emails. It stores the emails and sent the emails to other clients. If we want to send any mail we have to send it by use of the mail server.

**Proxy Server**  
The Proxy Server improve the performance between the client and the server. The different clients will access the same site at a time so it will increase the traffic. So the proxy server will route the traffic into another large network.

**Cloud Server**  
The Cloud Server provides the functionality that stores a huge amount of data without having physical memory. These servers are accessed through the application. If we don't have memory in the local storage then we buy the cloud storage and use that storage as the server.[  
](https://res.cloudinary.com/practicaldev/image/fetch/s--b_Jy2nv3--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9qp8dpaoo3jssjqi6i1k.png)

## Advantages of servers

* Scalability
    
* Faster
    
* Collaboration of different servers
    
* Secured