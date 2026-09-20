# Lecture 01 — Introduction to Software, Applications & Full Stack

> **Course:** Web Development
> **Batch:** SOT 26
> **Level:** Beginner / First-Time Learner

---

# 1. What is a Computer?

A **computer** is an electronic device that accepts data as input, processes that data, produces an output, and can store information for future use.

### Simple Example

Suppose you use a calculator:

```text
Input
  ↓
10 + 20
  ↓
Processing
  ↓
30
  ↓
Output
```

A computer basically performs four major activities:

```text
Input → Processing → Output → Storage
```

### Real-Life Examples of Computers

* Laptop
* Desktop
* Smartphone
* Tablet
* ATM
* Smart TV
* Smartwatch
* Server

---

# 2. Computer System = Hardware + Software

A computer system has two fundamental parts:

```text
             COMPUTER SYSTEM
                    │
          ┌─────────┴─────────┐
          ↓                   ↓
      HARDWARE             SOFTWARE
```

Both are required for a computer system to work properly.

---

# 3. What is Hardware?

**Hardware** refers to the physical components of a computer that we can see and touch.

### Examples

* Keyboard
* Mouse
* Monitor
* CPU
* RAM
* SSD
* Printer
* Webcam
* Speakers
* Graphics Card

### Simple Definition

> **Hardware is the physical part of a computer system.**

### Example

Consider a laptop:

```text
Laptop
│
├── Screen
├── Keyboard
├── Touchpad
├── RAM
├── SSD
├── Processor
└── Battery
```

All of these are hardware components.

---

# 4. What is Software?

**Software** is a set of instructions or programs that tells a computer what to do.

Unlike hardware, software cannot be physically touched.

### Examples

* Windows
* Linux
* Google Chrome
* Microsoft Word
* VS Code
* WhatsApp
* Games
* Photoshop

### Simple Definition

> **Software is a set of instructions that tells hardware how to perform a task.**

### Hardware + Software Example

Suppose you want to watch a YouTube video.

```text
        You
         ↓
      YouTube
         ↓
      Browser
         ↓
    Operating System
         ↓
      Hardware
         ↓
 Screen + Speakers
```

The hardware performs the physical work, while the software provides the instructions.

---

# 5. What is an Application?

Now that we understand hardware and software, let's understand an important concept:

> **Application**

An **application** is a software program designed to help users perform a particular task or a group of related tasks.

### Examples

| Application   | Purpose               |
| ------------- | --------------------- |
| Calculator    | Perform calculations  |
| Google Chrome | Browse the internet   |
| WhatsApp      | Communication         |
| MS Word       | Create documents      |
| Spotify       | Listen to music       |
| Amazon        | Online shopping       |
| Instagram     | Social networking     |
| VS Code       | Write and manage code |

### Simple Understanding

```text
Software
   ↓
Application
   ↓
Helps user perform a task
```

For example:

```text
Calculator
    ↓
Perform calculations

WhatsApp
    ↓
Communicate with people

Amazon
    ↓
Buy products
```

Applications can be created for different platforms and purposes.

---

# 6. Types of Applications

Applications can be developed in many different forms.

In this lecture, we will understand:

```text
Applications
│
├── Desktop Applications
├── Web Applications
├── Distributed Applications
├── Mobile Applications
├── AI Applications
├── IoT Applications
└── 2D & 3D Applications
```

---

# 7. Desktop Applications

## What is a Desktop Application?

A **desktop application** is an application that is installed and runs directly on a desktop computer or laptop.

### Examples

* Microsoft Word
* VLC Media Player
* Photoshop
* Visual Studio Code
* Calculator
* Adobe Premiere Pro

### How does it work?

```text
Computer
   ↓
Install Application
   ↓
Run Application
   ↓
Use Application
```

For example, when you install VS Code on your laptop, the application runs on your computer.

---

## Advantages of Desktop Applications

### 1. Can work offline

Many desktop applications can work without an internet connection.

Example:

> You can use Calculator without internet.

### 2. High performance

Desktop applications can directly use the computer's resources such as:

* CPU
* RAM
* GPU
* Storage

This can make them suitable for resource-intensive tasks.

### 3. Access to system resources

Desktop applications can often interact closely with the operating system and hardware.

For example:

* File system
* Printer
* Camera
* GPU
* Local storage

### 4. Can provide rich features

Applications such as Photoshop and video editing software can provide powerful functionality.

---

## Disadvantages of Desktop Applications

### 1. Installation is required

Users usually need to download and install the application.

### 2. Platform dependency

An application may need separate versions for:

```text
Windows
macOS
Linux
```

### 3. Updates may need installation

Users may need to download updates or install new versions.

### 4. Device dependency

The application generally runs on the device where it is installed.

---

# 8. Web Applications

## What is a Web Application?

A **web application** is an application that users access through a web browser over a network, commonly the internet.

### Examples

* Gmail
* YouTube
* Google Docs
* Amazon
* Netflix
* Online Banking
* GitHub

### Basic Flow

```text
User
 ↓
Web Browser
 ↓
Internet / Network
 ↓
Web Server
 ↓
Application
```

## Advantages of Web Applications

### 1. No traditional installation required

Users can generally access the application through a browser.

```text
Open Browser
     ↓
Enter Website
     ↓
Use Application
```

### 2. Cross-platform

A web application can usually be accessed from different operating systems if a compatible browser is available.

For example:

```text
Windows
macOS
Linux
Android
iOS
```

### 3. Easy updates

Updates can be deployed on the server.

Users generally don't have to manually install a new version of the application.

### 4. Easy accessibility

Users can access the application from different devices, depending on the application's design and requirements.

### 5. Centralized data

Data and application logic can be managed centrally on servers.

---

## Disadvantages of Web Applications

### 1. Internet/network dependency

Many web applications require an internet or network connection.

### 2. Browser dependency

The application needs to work correctly with supported browsers.

### 3. Performance limitations

Some operations may be affected by:

* Network speed
* Server performance
* Browser limitations

### 4. Security risks

Because web applications are connected to networks, developers need to carefully handle:

* Authentication
* Authorization
* Data protection
* Input validation
* Common web security threats

---

# 9. Desktop Application vs Web Application

| Feature      | Desktop Application      | Web Application          |
| ------------ | ------------------------ | ------------------------ |
| Installation | Usually required         | Usually not required     |
| Runs on      | Computer                 | Web browser              |
| Internet     | May not be required      | Often required           |
| Updates      | May require installation | Usually server-side      |
| Platform     | Often OS-specific        | Generally cross-platform |
| Example      | Photoshop                | Google Docs              |

### Easy Way to Remember

```text
Desktop Application
        ↓
Installed on Computer

Web Application
        ↓
Accessed through Browser
```

---

# 10. Distributed Applications

## What is a Distributed Application?

A **distributed application** is an application in which different components or services work across multiple computers or systems and communicate with each other over a network.

Instead of everything running on one computer, different parts may run on different machines.

### Example

Consider an online shopping application:

```text
          User
           ↓
        Browser
           ↓
      Web Server
           ↓
    Application Server
       ↙    ↓     ↘
 Database  Payment  Other Services
```

Different components work together to provide the complete application.

### Let's talk about Zomato

Now, let's take a real-life example of a **distributed application — Zomato**.

Suppose there is a person, let's call him **X**, and X is using Zomato. He opens Zomato, selects a restaurant, chooses some food, and places an order.

Now, after placing the order, X needs to make the payment.

So, when X goes to the payment section, what happens?

A **Payment Gateway** opens.

This Payment Gateway could be provided by **Paytm, Razorpay, Stripe, Cashfree**, or any other payment provider.

Now, notice one important thing here.

**Zomato is one entity, and the Payment Gateway is another entity.**

For example, suppose Zomato is using Razorpay for payments.

The flow would look something like this:

```text
User
  ↓
Zomato
  ↓
Payment Gateway
  ↓
Bank / UPI / Card Network
```

The user is using Zomato, but Zomato is communicating with another independent system to complete the payment.

And this is where the concept of a **distributed application** comes in.

The different systems are independent, but they communicate with each other over a network and work together to complete one common task.

Now you might ask:

**"Why doesn't Zomato simply build its own Payment Gateway from scratch?"**

Technically, a large company can build its own payment infrastructure, but it is not just about creating one small feature.

A payment system requires many things:

* Integration with banks and payment networks
* Strong security
* Fraud detection
* Payment processing infrastructure
* Compliance and regulations
* Refund handling
* Failed transaction handling
* Secure transaction management

If Zomato started building all of this from zero, it would have to move beyond its **core business of food delivery** and build and maintain an entire payment infrastructure.

Instead, Zomato can use a specialized Payment Gateway and integrate it into its application.

So now we have:

```text
        ZOMATO
          |
          | Network Communication
          ↓
   PAYMENT GATEWAY
          |
          ↓
    BANK / UPI / CARD
```

Zomato and the Payment Gateway are **separate systems**, but they communicate with each other and work together to complete the user's request.

That's the basic idea behind a **distributed application**:

> **Different independent systems or components communicate over a network and work together to provide a common service.**


---

## Examples

* Online banking systems
* E-commerce platforms
* Cloud applications
* Large social media platforms
* Video streaming platforms
* Enterprise systems

---

## Advantages of Distributed Applications

### 1. Scalability

Different components can be scaled independently.

For example:

```text
More Users
    ↓
Add More Application Servers
```

### 2. Better resource utilization

Different systems can handle different responsibilities.

### 3. Reliability

If designed properly, some components can continue operating even when another component has a problem.

### 4. Separation of responsibilities

Different services can perform different tasks.

For example:

```text
Authentication Service
Payment Service
Notification Service
Order Service
```

---

## Disadvantages of Distributed Applications

### 1. Complexity

There are multiple components that need to communicate with each other.

### 2. Network dependency

Communication between components usually happens over a network.

### 3. Debugging is harder

Finding the source of a problem can be more difficult because multiple systems are involved.

### 4. Security becomes more important

More communication points mean more areas that need to be secured.

---

# 11. Mobile Applications

## What is a Mobile Application?

A **mobile application** is software designed primarily for mobile devices such as smartphones and tablets.

### Examples

* WhatsApp
* Instagram
* Google Maps
* Spotify
* PhonePe
* Uber

### Major Mobile Platforms

```text
Android
iOS
```

---

## Advantages of Mobile Applications

### 1. Portability

Users can carry their mobile devices almost everywhere.

### 2. Device features

Mobile applications can use device capabilities such as:

* Camera
* GPS
* Microphone
* Bluetooth
* Sensors
* Notifications

### 3. Better mobile experience

Applications can be specifically designed for touch screens and mobile devices.

### 4. Notifications

Mobile applications can provide push notifications to users.

---

## Disadvantages of Mobile Applications

### 1. Installation required

Users generally need to install the application.

### 2. Platform differences

Android and iOS applications may require different development approaches.

### 3. Storage consumption

Applications can consume:

* Storage
* RAM
* Battery
* Mobile data

### 4. Regular updates

Users may need to update the application to receive new features or fixes.

---

# 12. AI Applications

## What is an AI Application?

An **AI application** uses Artificial Intelligence techniques to perform tasks that traditionally require capabilities such as pattern recognition, prediction, language understanding, or decision-making.

### Examples : ChatGPT , Grok , Copilot etc

* Chatbots
* AI assistants
* Recommendation systems
* Image recognition systems
* Voice assistants
* AI coding tools
* Fraud detection systems

---

## Simple AI Application Flow

```text
Input Data
    ↓
AI Model
    ↓
Processing / Prediction
    ↓
Result
```

Example:

```text
User asks a question
        ↓
AI Model
        ↓
Processes the question
        ↓
Generates a response
```

---

## Advantages of AI Applications

### 1. Automation

AI can automate repetitive or complex tasks.

### 2. Fast processing

AI systems can process large amounts of data quickly.

### 3. Personalization

AI can provide personalized recommendations and experiences.

### 4. Pattern recognition

AI can identify patterns in large datasets.

---

## Disadvantages of AI Applications

### 1. Data dependency

Many AI systems require suitable and sufficient data.

### 2. Incorrect results

AI systems can sometimes produce incorrect or unreliable results.

### 3. Cost

Developing and operating advanced AI systems can require significant computing resources.

### 4. Privacy concerns

Applications that process personal or sensitive data need appropriate privacy and security controls.

---

# 13. IoT Applications

## What is IoT?

**IoT** stands for:

> **Internet of Things**

IoT refers to physical devices that can collect data, communicate over a network, and sometimes perform actions based on that data.

### Examples

* Smart watch
* Smart bulb
* Smart TV
* Smart security camera
* Smart thermostat
* Industrial sensors
* Smart agriculture systems

---

## Example: Smart Home

```text
Smart Bulb
     ↓
Internet
     ↓
Cloud / Server
     ↓
Mobile Application
     ↓
User
```

The user can control the smart bulb using a mobile application.

---

## Advantages of IoT Applications

### 1. Automation

Devices can perform actions automatically.

### 2. Remote monitoring

Users can monitor devices remotely.

### 3. Real-time data

Sensors can continuously collect information.

### 4. Better efficiency

IoT can help organizations monitor resources and automate processes.

---

## Disadvantages of IoT Applications

### 1. Security risks

Connected devices can become targets for attacks if not properly secured.

### 2. Internet dependency

Many IoT systems depend on network connectivity.

### 3. Privacy concerns

Devices may collect large amounts of information about users or environments.

### 4. Maintenance

Devices, sensors, networks, and software need maintenance and updates.

---

# 14. 2D and 3D Applications

## What are 2D Applications?

2D applications work with two-dimensional content such as:

```text
Width
Height
```

### Examples

* 2D games
* Drawing applications
* Image editors
* 2D animation software

---

## What are 3D Applications?

3D applications work with three-dimensional objects and environments.

```text
Width
Height
Depth
```

### Examples

* 3D games
* 3D modelling
* Animation
* Architecture visualization
* Simulations
* Virtual Reality

### Technologies / Tools

* Unity
* Unreal Engine
* Canva
* Paint
* DaVinci
* Blender
* OpenGL
---

## Advantages of 2D and 3D Applications

### 1. Visualization

Complex concepts can be represented visually.

### 2. Interactive experiences

Users can interact with objects and environments.

### 3. Entertainment

Used heavily in:

* Games
* Movies
* Animation
* Virtual Reality

### 4. Simulation

3D environments can be used for training and simulation.

---

## Disadvantages of 2D and 3D Applications

### 1. Development complexity

Advanced applications can require specialized skills.

### 2. Hardware requirements

High-quality 3D applications may require powerful hardware.

### 3. Development cost

Complex graphics and simulations can require significant development time and resources.

### 4. Large application size

Graphics-heavy applications can require considerable storage.

---

# 15. Comparison of Application Types

| Application Type | Example                        | Main Platform / Environment             |
| ---------------- | ------------------------------ | --------------------------------------- |
| Desktop          | VS Code, Photoshop             | Computer                                |
| Web              | Gmail, Amazon                  | Browser                                 |
| Distributed      | Banking System                 | Multiple Systems                        |
| Mobile           | WhatsApp, Instagram            | Smartphone                              |
| AI               | Chatbot, Recommendation System | Various                                 |
| IoT              | Smart Home                     | Connected Devices                       |
| 2D/3D            | Games, Blender                 | Computer / Mobile / Specialized Devices |

---

# 16. Where Does Web Development Fit?

We have now seen many types of applications.

Our main focus in this course is:

> **Web Applications**

To build web applications, we need to understand **Web Development**.

---

# 17. What is Web Development?

**Web development** is the process of creating and maintaining websites and web applications.

A modern web application commonly contains:

```text
Frontend
   +
Backend
   +
Database
```

These components work together to create a complete application.

---

# 18. Frontend

The **frontend** is the part of a web application that users can see and interact with.

### Examples

* Buttons
* Forms
* Images
* Navigation bars
* Cards
* Tables
* Menus
* Animations

### Basic Frontend Technologies

```text
HTML
 ↓
Structure

CSS
 ↓
Design

JavaScript
 ↓
Logic + Interactivity
```

---

# 19. HTML

**HTML** stands for:

> **HyperText Markup Language**

HTML is used to create the structure of a webpage.

For example:

```text
Heading
Paragraph
Image
Button
Form
Table
```

Think of HTML as the **structure/skeleton** of a webpage.

---

# 20. CSS

**CSS** stands for:

> **Cascading Style Sheets**

CSS is used to style webpages.

CSS controls:

* Colors
* Fonts
* Spacing
* Size
* Layout
* Borders
* Animations
* Responsive design

Think of CSS as the **design and appearance** of the webpage.

---

# 21. JavaScript

**JavaScript** is a programming language used to add logic and interactivity to web applications.

Example:

```text
User clicks button
       ↓
JavaScript
       ↓
Perform an action
```

JavaScript can be used to:

* Handle events
* Validate forms
* Change webpage content
* Fetch data
* Communicate with APIs
* Build interactive applications

---

# 22. Backend

The **backend** is the part of an application that works behind the scenes.

Backend responsibilities may include:

* Business logic
* Authentication
* Authorization
* APIs
* Processing requests
* Database communication
* Server-side operations

### Example

When a user logs in:

```text
Frontend
   ↓
Login Request
   ↓
Backend
   ↓
Check User Details
   ↓
Database
   ↓
Backend
   ↓
Response
   ↓
Frontend
```

---

# 23. Database

A **database** is a system used to store and manage data.

For an e-commerce application, the database may contain:

```text
Users
Products
Orders
Payments
Addresses
Reviews
```

Basic architecture:

```text
Frontend
    ↓
Backend
    ↓
Database
```

---

# 24. Full Stack Development

**Full Stack Development** refers to working with multiple layers of a web application, commonly including:

```text
Frontend
   +
Backend
   +
Database
```

A simplified architecture:

```text
                 USER
                   ↓
             ┌───────────┐
             │ FRONTEND  │
             │ HTML CSS  │
             │ JavaScript│
             │   React   │
             └─────┬─────┘
                   ↓
                 API
                   ↓
             ┌───────────┐
             │  BACKEND  │
             │ Node/Java │
             │  Python   │
             └─────┬─────┘
                   ↓
             ┌───────────┐
             │ DATABASE  │
             │MySQL/Mongo│
             └───────────┘
```

---

# 25. Full Stack Career

A Full Stack Developer generally works across multiple areas.

## Frontend Technologies

Examples:

```text
HTML
CSS
JavaScript
React
```

### Focus

* User Interface
* User Experience
* Browser
* Responsiveness
* Interaction

---

## Backend Technologies

Examples:

```text
Node.js
Express.js
Java
Spring Boot
Python
Django
```

### Focus

* Server
* APIs
* Business Logic
* Authentication
* Data Processing

---

## Database

Examples:

```text
MySQL
PostgreSQL
MongoDB
```

### Focus

* Data Storage
* Queries
* Relationships
* CRUD
* Data Management

---

