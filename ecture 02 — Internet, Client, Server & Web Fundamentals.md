# Lecture 02 — Internet, Client, Server & Web Fundamentals
---

# 1. What is a Client?

A **client** is a device or application that requests a service or resource from another computer.

### Simple Example

When you open Google Chrome and search for something:

Here, your browser(Google Chrome) acts as a **client**.

### Examples of Clients

* Web Browser
* Mobile Application
* Desktop Application
* Email Application

### Real-Life Example

Think about a restaurant.

```text
Customer → Waiter → Kitchen
```

The **customer** asks for something. So the customer is the **client**.

Similarly:

```text
Client → Server
```

The client asks the server for something.

---

# 2. What is a Server?

A **server** is a computer or software system that provides services, resources, or data to clients over a network.

### Simple Example

You open:

```text
www.google.com
```

Your browser sends a request to Google's servers.

The server processes the request and sends a response back.

```text
Client
  ↓
Request
  ↓
Server
  ↓
Response
  ↓
Client
```

### What can a Server provide?

A server can provide:

* Web pages
* Images
* Videos
* Files
* Data
* APIs
* Emails
* Authentication services

---

# 3. Client vs Server

| Client                                   | Server                          |
| ---------------------------------------- | ------------------------------- |
| Requests a service                       | Provides a service              |
| Usually interacts directly with the user | Usually works behind the scenes |
| Sends requests                           | Receives requests               |
| Receives responses                       | Sends responses                 |
| Example: Browser                         | Example: Web Server             |

### Simple Example

When you open an online shopping website:

```text
Your Browser
    ↓
   Client
    ↓
 Request
    ↓
   Server
    ↓
 Response
    ↓
Your Browser
```

This means you ask the server for the website, and the server sends it back to you.

---

# 5. What is the Internet?

The **Internet** is a global network of interconnected computer networks that communicate with each other.

In simple words:

> **The Internet is a network of networks.**

It connects billions of devices around the world.

### Example

Your laptop can communicate with a server located in another country through the Internet.

# 6. What is a Network?

A **network** is a group of connected devices that can communicate and share information.

### Example

Suppose a college has:

```text
Computer 1 ─┐
Computer 2 ─┤
Computer 3 ─┼── Network
Computer 4 ─┤
Printer ────┘
```

These devices can communicate with each other.

---

# 7. Internet vs Network

These two terms are related but not exactly the same.

### Network

A network connects a group of devices.

Example:

> Computers connected inside a college.

### Internet

The Internet connects networks around the world.

```text
Local Network
      ↓
     ISP
      ↓
   Internet
      ↓
Other Networks
```

### Remember

> **A network can exist without being connected to the global Internet.**

---

# 8. Fundamentals of the Internet

To understand web development, we need to understand a few basic Internet concepts.

```text
Device
  ↓
Network
  ↓
Router
  ↓
ISP
  ↓
Internet
  ↓
Server
```

Let's understand these one by one.

---

## 8.1 Device

A device is something that connects to a network.

Examples:

* Laptop
* Smartphone
* Desktop
* Server
* Smart TV
* IoT device

---

## 8.2 Router

A **router** is a networking device that forwards data between networks.

For example:

```text
Your Laptop
     ↓
Wi-Fi Router
     ↓
Internet
```

Your router helps your devices communicate with other networks.

---

## 8.3 ISP

ISP stands for:

> **Internet Service Provider**

An ISP provides Internet connectivity to users and organizations.

Examples include Internet providers such as:

* Airtel
* Jio
* BSNL

---

# 9. What is the Web?

The **World Wide Web (WWW)** is a system of interconnected web resources that we access over the Internet using web technologies and protocols.

### Important

> **Internet and Web are not the same thing.**

The Internet is the underlying global network.

The Web is one of the services that operates over the Internet.

### Simple Example

```text
INTERNET
│
├── World Wide Web
├── Email
├── File Transfer
├── Online Communication
└── Other Services
```

So:

> **Web is a service that runs on the Internet.**

---

# 10. Website vs Web Application

A **website** primarily provides information or content to users.

Examples:

* News websites
* College information websites
* Documentation websites

A **web application** allows users to interact with the system and perform tasks.

Examples:

* Gmail
* Google Docs
* Online Banking
* E-commerce applications

### Simple Difference

```text
Website
↓
Mostly consume information

Web Application
↓
Interact + perform tasks
```

The distinction is not always strict because modern websites often contain application-like functionality.

---

# 11. How Does a Web Page Reach Your Browser?

Suppose you type:

```text
www.example.com
```

into your browser.

What happens?

A simplified flow is:

```text
You
 ↓
Browser
 ↓
Find Server
 ↓
Send Request
 ↓
Server
 ↓
Process Request
 ↓
Send Response
 ↓
Browser
 ↓
Display Web Page
```

Let's understand this process step by step.

---

# 12. Step 1 — User Enters a URL

Suppose you enter:

```text
https://example.com
```

The browser needs to find the appropriate server.

---

# 13. Step 2 — Domain Name

Humans prefer names such as:

```text
google.com
amazon.com
github.com
```

Computers communicate using network addresses such as IP addresses.

This is where **DNS** becomes important.

### DNS

DNS stands for:

> **Domain Name System**

DNS helps translate a domain name into an IP address.

Conceptually:

```text
google.com
     ↓
    DNS
     ↓
IP Address
```

This allows the client to locate the appropriate server.

---

# 14. Step 3 — Client Sends a Request

Once the client knows where to communicate, it sends a request.

For a web request, the browser commonly uses **HTTP or HTTPS**.

Simplified:

```text
Browser
   ↓
HTTP/HTTPS Request
   ↓
Server
```

---

# 15. Step 4 — Server Receives the Request

The server receives the request and determines what needs to be done.

For example:

```text
GET /products
```

The server may:

```text
Receive Request
      ↓
Process Request
      ↓
Check Application Logic
      ↓
Access Database if Required
      ↓
Prepare Response
```

---

# 16. Step 5 — Server Sends a Response

After processing the request, the server sends a response back to the client.

```text
Client
   ↓
Request
   ↓
Server
   ↓
Response
   ↓
Client
```

The response may contain:

* HTML
* CSS
* JavaScript
* JSON
* Images
* Videos
* Other resources

---

# 17. Step 6 — Browser Displays the Result

The browser receives the response and processes it.

For example:

```text
HTML
 ↓
Create Page Structure

CSS
 ↓
Apply Styling

JavaScript
 ↓
Add Interactivity
```

Finally, the browser displays the webpage to the user.

---

# 18. Complete Request-Response Flow


```text
┌──────────┐       Network        ┌──────────┐
│  Client  │ ─── Request ───────→ │  Server  │
│          │ ←── Response ─────── │          │
└──────────┘                       └──────────┘
```

**Client → Request → Server**

**Client ← Response ← Server**


---

# 19. What is a Protocol?

A **protocol** is a set of rules that defines how devices communicate with each other.

Think of a protocol like a common language or agreed set of rules.

### Real-Life Example

When two people communicate:

```text
Person A
   ↓
Language / Rules
   ↓
Person B
```

Computers also need agreed rules.

```text
Computer A
    ↓
 Protocol
    ↓
Computer B
```

---

# 20. HTTP

HTTP stands for:

> **HyperText Transfer Protocol**

HTTP is a protocol used for communication between web clients and web servers.

Basic communication:

```text
Client
  ↓
HTTP Request
  ↓
Server
  ↓
HTTP Response
  ↓
Client
```

---

# 21. HTTPS

HTTPS stands for:

> **HyperText Transfer Protocol Secure**

HTTPS provides HTTP communication with encryption through TLS.

You commonly see:

```text
https://
```

instead of:

```text
http://
```

HTTPS helps protect data while it is transmitted between the client and server.

---

# 22. SMTP

SMTP stands for:

> **Simple Mail Transfer Protocol**

SMTP is used for **sending email messages** between mail systems.

SMTP is mainly associated with **sending and relaying email**.

---

# 23. FTP

FTP stands for:

> **File Transfer Protocol**

FTP is used to transfer files between computers over a network.

A user can transfer files such as:

* Images
* Documents
* Videos
* Website files

### FTP Operations

FTP can support operations such as:

```text
Upload
Download
Rename
Delete
List Files
```

### Important

FTP is an older protocol and does not encrypt the entire communication by default.

More secure alternatives include:

* SFTP
* FTPS

---

# 25. What is an IP Address?

IP stands for:

> **Internet Protocol**

An **IP address** is a numerical address used to identify a device or network interface on an IP network.

Think of it like an address used for network communication.

### Simple Example

Instead of remembering:

```text
Server Name
```

network communication uses an IP address such as:

```text
192.168.1.10
```

---

# 26. Why Do We Need IP Addresses?

Imagine a city where every house has no address.

How would a delivery person know where to deliver a package?

Similarly, computers need addresses so that data can be delivered to the correct destination.


# 29. Public IP vs Private IP

## Private IP

Used within private networks such as:

* Home networks
* College networks
* Office networks

Example:

```text
192.168.1.10
```

## Public IP

A public IP address is used for communication across the public Internet.

Your router/network may have a public IP assigned by your Internet provider.

### Simple Picture

```text
Laptop
  ↓
Private IP
  ↓
Router
  ↓
Public IP
  ↓
Internet
```

---

# 30. What is a Request?

A **request** is a message sent by a client to a server asking the server to perform an action or provide a resource.

Example:

```text
Client → "Give me the homepage."
```

The browser sends this request to the server.

---

# 31. What is a Response?

A **response** is the message sent by the server back to the client after processing a request.

```text
Client
  ↓
Request
  ↓
Server
  ↓
Response
  ↓
Client
```

Example:

```text
Request:
"Give me /home"

Response:
"Here is the requested page."
```

> **Next Lecture → How the Web Works: URL, DNS, HTTP/HTTPS, Ports, TCP/IP & Browser Request Flow**
