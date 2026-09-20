# Lecture 03 — Web Development Tools & Development Environment & HTML

---

# 1. What Do We Need to Start Web Development?

Before writing our first HTML, CSS, or JavaScript program, we need a proper environment where we can:

* Write code
* Save code
* Run code
* See the output
* Debug errors
* Manage our project files

For this, the first thing we need is a **Code Editor / IDE**.

---

# 2. What is an IDE / Code Editor?

An **IDE (Integrated Development Environment)** is a software application that provides tools for writing, running, testing, and managing code.

For beginners, you can think of it as:

> **A software where we write and manage our programming code.**

For Web Development, we commonly work with:

```text
HTML
CSS
JavaScript
```

So we need a good development environment to work with these technologies.

### Simple Example

Instead of writing HTML in a normal text editor:

```text
Notepad
```

we can use a modern development tool:

```text
VS Code
```

which provides features specifically useful for developers.

---

# 3. Popular IDEs / Code Editors for Web Development

There are many tools available for HTML, CSS, and JavaScript development.

Some popular options are:

| Tool               | Company / Organization | Common Use                   |
| ------------------ | ---------------------- | ---------------------------- |
| Visual Studio Code | Microsoft              | Web & general development    |
| WebStorm           | JetBrains              | JavaScript / Web Development |
| Sublime Text       | Sublime HQ             | Code editing                 |
| IntelliJ IDEA      | JetBrains              | Java + Web Development       |
| Vim / Neovim       | Open Source Community  | Advanced code editing        |
| Eclipse            | Eclipse Foundation     | Java + Web Development       |
| Brackets           | Open Source            | Web Development              |
| Notepad++          | Don Ho                 | Lightweight code editing     |
| Cursor             | Anysphere              | AI-assisted development      |
| Zed                | Zed Industries         | Modern code editing          |

> **Note:** The best tool can depend on the developer, project, operating system, and workflow. For this course, we will standardize on **Visual Studio Code**.

---

# 4. Why Are We Using VS Code?

For this course, we will use:

> **Visual Studio Code (VS Code)**

VS Code is a source-code editor that supports many programming languages and development workflows.

### Why are we choosing VS Code?

## 4.1 Free to Use

VS Code is available free of charge.

---

## 4.2 Supports Web Technologies

We can easily work with:

```text
HTML
CSS
JavaScript
JSON
Node.js
React
```

and many other technologies.

---

## 4.3 Extensions

VS Code has an extensive extension ecosystem.

We can add features according to our requirements.

For example:

```text
VS Code
   ↓
Install Extension
   ↓
Additional Functionality
```

---

## 4.4 Integrated Terminal

We can run commands directly inside VS Code.

For example:

```bash
node -v
npm -v
```

and later:

```bash
npm install
```

---

## 4.5 Project Management

VS Code makes it easy to work with folders and multiple files.

Example:

```text
my-project/
│
├── index.html
├── style.css
└── script.js
```

---

## 4.6 Git Support

VS Code provides built-in support for working with Git repositories.

This will become useful when we start working with **Git and GitHub**.

---

# 5. Download and Install VS Code

We will now install VS Code on our computer.

### Step 1 — Open the Official Website

Search for:

> **Visual Studio Code**

Always download VS Code from the official website.

### Step 2 — Choose Your Operating System

VS Code provides installers for major operating systems such as:

```text
Windows
macOS
Linux
```

Choose the version according to your operating system.

### Step 3 — Install

After downloading:

1. Open the installer.
2. Follow the installation instructions.
3. Complete the installation.
4. Open VS Code.

After installation, you should see the VS Code interface.

---

# 6. Understanding the VS Code Interface

When you open VS Code, you will see several important areas.

```text
┌─────────────────────────────────────────┐
│               VS CODE                   │
├──────────┬──────────────────────────────┤
│          │                              │
│ Explorer │                              │
│ Search   │          Editor              │
│ Source   │                              │
│ Control  │                              │
│ Run      │                              │
│Extensions│                              │
│          │                              │
├──────────┴──────────────────────────────┤
│              Terminal                   │
└─────────────────────────────────────────┘
```

The most important areas for now are:

* **Explorer** → Manage files and folders
* **Editor** → Write code
* **Extensions** → Install extensions
* **Terminal** → Run commands

---

# 7. What are VS Code Extensions?

An **extension** is an additional software component that adds functionality to VS Code.

Think of VS Code as your basic development environment.

You can then add features when you need them.

```text
VS Code
   +
Extension
   ↓
Additional Feature
```

For our Web Development course, we will start with extensions that make running and previewing webpages easier.

---

# 8. Live Server Extension

One useful extension for beginners is:

> **Live Server**

Live Server can start a local development server for your project and automatically refresh the browser when supported files are changed.

---

# 9. Why Do We Need Live Server?

Suppose we create:

```text
index.html
```

and write:

```html
<h1>Hello World</h1>
```

We want to see the result in the browser.

We could open the HTML file directly.

But during development, repeatedly refreshing and managing local files manually becomes inconvenient.

Live Server gives us a development workflow like:

```text
Write Code
    ↓
Save File
    ↓
Local Server
    ↓
Browser
    ↓
Updated Page
```

This makes learning and development more convenient.

---

# 10. How to Install Live Server

### Step 1

Open VS Code.

### Step 2

Click the:

> **Extensions**

icon from the left sidebar.

### Step 3

Search for:

```text
Live Server
```

### Step 4

Select the appropriate extension.

### Step 5

Click:

> **Install**

After installation, you can use Live Server with your HTML project.

---

# 11. Running a Web Page Using Live Server

Suppose our project contains:

```text
my-website/
└── index.html
```

Open the project folder in VS Code.

Then open `index.html`.

You can start the page using the Live Server command, commonly available as:

> **Open with Live Server**

The browser will open the webpage through a local server.

You may see an address similar to:

```text
http://127.0.0.1:5500/
```

or:

```text
http://localhost:5500/
```

The exact port may vary.

---

# 12. Live Preview

Another useful VS Code extension/tool is:

> **Live Preview**

It can provide a live preview of web pages while you work.

The basic idea is:

```text
Code
 ↓
Preview
 ↓
See Result
```

This is especially useful while learning HTML and CSS because students can immediately connect:

```text
Code
 ↓
Output
```

---

# 13. Live Server vs Live Preview

Both tools can help us see our webpage while developing.

| Live Server                       | Live Preview                                   |
| --------------------------------- | ---------------------------------------------- |
| Starts a local development server | Provides a live preview workflow               |
| Opens the page in a browser       | Can preview within the development environment |
| Useful for browser-based testing  | Useful for quick development preview           |
| Common beginner workflow          | Convenient inside VS Code                      |

For this course, students may use either depending on the workflow being demonstrated.

---

# 14. Now We Need Node.js

So far, we have:

```text
VS Code
   ↓
HTML / CSS / JavaScript
```

But there is another important tool we need.

> **Node.js**

---

# 15. What is Node.js?

**Node.js is a JavaScript runtime that allows JavaScript to run outside a web browser.**

Normally, when we think about JavaScript, we often think about:

```text
JavaScript
    ↓
Browser
```

Node.js allows JavaScript to run in environments outside the browser.

```text
JavaScript
    ↓
Node.js
    ↓
Operating System
```

---

# 16. Why Are We Installing Node.js?

For our course, one important reason is:

> **Node.js comes with npm, the Node Package Manager.**

We will use npm to install and manage packages required by our projects.

Later, Node.js will also become important when we learn **backend development**.

So Node.js is useful for us both now and later.

---

# 17. Downloading Node.js

Go to the official Node.js website.

Download the appropriate version for your operating system.

For most students:

```text
Windows → Windows Installer
macOS   → macOS Installer
Linux   → Linux installation method
```

Follow the installation instructions.

After installation, open a terminal.

---

# 18. Verify Node.js Installation

Open the VS Code terminal.

You can open it from:

```text
Terminal → New Terminal
```

Then run:

```bash
node -v
```

If Node.js is installed correctly, you will see a version number.

For example:

```text
v22.x.x
```

The exact version may be different depending on the current Node.js release.

---

# 19. What is npm?

When Node.js is installed, npm is normally installed along with it.

npm stands for:

> **Node Package Manager**

npm is used to:

* Install packages
* Remove packages
* Update packages
* Manage dependencies
* Run project scripts

---

# 20. Check npm Installation

In the VS Code terminal, run:

```bash
npm -v
```

If npm is installed correctly, it will display a version number.

For example:

```text
10.x.x
```

Again, the exact version may vary.

---

# 21. Why Do We Need Packages?

This is a very important question.

Imagine we are building a website.

We need:

* Buttons
* Forms
* Responsive layouts
* Icons
* Animations
* Components
* Utilities

Should we build **everything from zero**?

Not necessarily.

Developers frequently reuse existing libraries and packages.

```text
Our Project
     ↓
Existing Package
     ↓
Use Its Functionality
```

---

# 22. Why Don't We Build Everything From Scratch?

Suppose we want a responsive CSS framework.

We could write:

```text
All CSS
 ↓
Grid System
 ↓
Buttons
 ↓
Cards
 ↓
Forms
 ↓
Responsive Design
 ↓
Utilities
```

But creating and maintaining all of this ourselves would take significant time.

Instead, we can use an existing framework such as:

> **Bootstrap**

Bootstrap provides reusable CSS and JavaScript components and utilities that can help developers build responsive interfaces more quickly.

---

# 24. Installing a Package Using npm

Suppose we want to use Bootstrap in a project.

First, we create/open our project folder.

Then we can initialize an npm project:

```bash
npm init -y
```

This creates:

```text
package.json
```

Now we can install Bootstrap:

```bash
npm install bootstrap
```

npm will download Bootstrap into our project.

---

# 25. What Happens When We Run `npm install`?

When we execute:

```bash
npm install bootstrap
```

npm:

```text
Reads Project
     ↓
Finds Package
     ↓
Downloads Package
     ↓
Installs Package
     ↓
Updates package.json
     ↓
Creates / Updates node_modules
```

The project may now look like:

```text
my-project/
│
├── node_modules/
│
├── package.json
│
├── package-lock.json
│
└── index.html
```

---

# 26. What is `node_modules`?

`node_modules` is the directory where npm installs project dependencies.

For example:

```text
my-project/
│
├── node_modules/
│   └── bootstrap/
│
├── package.json
└── package-lock.json
```

We generally do not manually edit the contents of `node_modules`.

---

# 27. What is `package.json`?

`package.json` is an important file in a Node.js/npm project.

It contains project metadata and information about dependencies and scripts.

For example:

```json
{
  "name": "my-project",
  "version": "1.0.0",
  "dependencies": {
    "bootstrap": "^5.x.x"
  }
}
```

# 1. What is a Website?

A **website** is a collection of related web pages and other resources that are available on the Web and are usually accessed through a domain name.

For example:

```text
google.com
youtube.com
instagram.com
amazon.com
```

A website can contain:

* Web pages
* Images
* Videos
* CSS files
* JavaScript files
* Fonts
* Documents
* APIs
* Other resources

---

# 2. Website vs Web Page

These two terms are often confused.

## Web Page

A **web page** is an individual document/resource that is displayed in a web browser.

For example:

```text
example.com/about
```

can represent an individual page of a website.

## Website

A **website** is the complete collection of related pages and resources.

For example:

```text
                 WEBSITE
                    │
       ┌────────────┼────────────┐
       ↓            ↓            ↓
     Home         About       Contact
       │
       ↓
    Products
       │
       ├── Product 1
       ├── Product 2
       └── Product 3
```

### Easy Example

Think about a book:

```text
Book
 ↓
Website

Individual Page
 ↓
Web Page
```

A website can contain many web pages.

---

# 3. What Happens When We Open a Website?

Suppose we type:

```text
https://example.com
```

in our browser.

A simplified flow is:

```text
User
 ↓
Browser
 ↓
Request
 ↓
Web Server
 ↓
Website Resources
 ↓
Response
 ↓
Browser
 ↓
Web Page
```

The browser receives the required resources and renders them into what we see on the screen.

---

# 4. What is a Web Page?

A **web page** is a document that can be displayed in a web browser.

The primary language used to structure a web page is:

> **HTML — HyperText Markup Language**

A web page can also use:

```text
HTML
 +
CSS
 +
JavaScript
```

### Their basic responsibilities

```text
HTML
 ↓
Structure

CSS
 ↓
Presentation / Design

JavaScript
 ↓
Behavior / Interactivity
```

---

# 5. What is a Static Web Page?

Let's start with the simplest type of web page.

> **Static Web Page**

A static web page contains predefined content that is generally delivered to the browser in the same form for a given resource.

# 6. Simple Example of a Static Page

Imagine we create a portfolio page:

```text
My Name
Web Developer

About Me

I am a Web Developer.

Skills:
HTML
CSS
JavaScript

Contact:
example@email.com
```

Suppose this information is written directly inside:

```text
index.html
```

Every visitor receives essentially the same predefined content.

```text
User A ──┐
         ├──→ index.html
User B ──┤
         │
User C ──┘
```

The file itself doesn't change based on which visitor requested it.

---

# 7. Real Examples of Static Websites

Static websites are commonly used when the content is mostly informational and doesn't need to be generated separately for every user.

Examples include:

* Personal portfolio websites
* Documentation websites
* Simple landing pages
* Company information pages
* Event information pages
* Simple blogs
* Project showcase websites

For example, a developer's portfolio might contain:

```text
Home
About
Skills
Projects
Contact
```

The information may remain the same for every visitor.

---

# 10. What is a Dynamic Web Page?

> **A dynamic web page is a page whose content can be generated or changed based on data, user input, request information, or other conditions.**

Instead of simply returning one fixed HTML file, the application can generate the response when it is needed.

---

# 11. Simple Example of a Dynamic Page

Imagine an e-commerce website.

# 12. Real Example — Amazon

Consider a large e-commerce platform such as:

[Amazon](https://www.amazon.in/)

Imagine the website has millions of products.

It would be impractical to manually create and maintain a completely separate hardcoded HTML page for every possible product.

When you open a particular product, the application can retrieve the relevant product data and display it.

Large websites commonly use this kind of dynamic architecture.

---

# 13. Real Example — Instagram

Consider:

[Instagram](https://www.instagram.com/)

When two users open Instagram, they don't necessarily see the same content.

For example:

```text
User A
 ↓
Posts from accounts A follows
 ↓
Recommendations for User A
```

while:

```text
User B
 ↓
Posts from accounts B follows
 ↓
Recommendations for User B
```

The content can depend on:

* Logged-in user
* Followed accounts
* Posts
* Likes
* Comments
* Recommendations
* User preferences
* Data stored on the server

Therefore, the application needs mechanisms to retrieve and generate user-specific content.

---

# 14. Real Example — YouTube

Consider:

[YouTube](https://www.youtube.com/)

Different users can receive different:

* Recommendations
* Subscriptions
* Watch history
* Search results
* Comments
* Playlists

The page is not simply one fixed HTML document containing all this information.

The application retrieves and displays data based on the user and request.

---

# 15. Static vs Dynamic — The Core Difference

> **Static = Content is already prepared.**

> **Dynamic = Content can be generated or changed based on data or conditions.**

---

# 16. Static vs Dynamic Example

Imagine a college website.

### Static Page

```text
About Our College

Established in 2020.

Our campus is located in Lucknow.

We offer B.Tech programs.
```

Every visitor sees the same information.

---

### Dynamic Page

Now imagine:

```text
Student Dashboard
```

Student A sees:

```text
Welcome Rahul

Attendance: 82%
Assignments: 8/10
Marks: 76%
```

Student B sees:

```text
Welcome Priya

Attendance: 91%
Assignments: 10/10
Marks: 88%
```

The structure may be similar, but the data is different.

That's a common example of dynamic content.

---

Modern websites often contain both static and dynamic parts.

For example, an e-commerce page might have:

```text
Static Structure
     ↓
Header
Navigation
Footer
Page Layout
```

and:

```text
Dynamic Data
     ↓
Product Name
Price
Stock
Reviews
Recommendations
```

So:

> **Modern websites are often a combination of static resources and dynamic content.**

---

# 20. Page Composition

Now that we understand what a web page is, let's understand:

> **How is a web page organized?**

A web page is usually divided into different logical sections.

For example:

```text
┌──────────────────────────────────┐
│              HEADER              │
├──────────────────────────────────┤
│            NAVIGATION            │
├──────────────────────────────────┤
│                                  │
│          HERO / BANNER           │
│                                  │
├──────────────────────────────────┤
│                                  │
│          MAIN CONTENT            │
│                                  │
│     ┌──────────┐ ┌──────────┐   │
│     │  Card 1  │ │  Card 2  │   │
│     └──────────┘ └──────────┘   │
│                                  │
├──────────────────────────────────┤
│             SIDEBAR              │
├──────────────────────────────────┤
│              FOOTER              │
└──────────────────────────────────┘
```

These sections together form the **composition** of the page.

---

# 21. Common Sections of a Web Page

## Header

Usually contains:

* Logo
* Website name
* Navigation
* User actions

Example:

```text
┌──────────────────────────────────┐
│ Logo     Home About Contact Login│
└──────────────────────────────────┘
```

---

## Navigation

Navigation helps users move between different pages or sections.

Example:

```text
Home | About | Services | Contact
```

---

## Hero Section

A hero section is usually a prominent section near the top of a page.

It may contain:

* Main heading
* Description
* Image
* Call-to-action button

Example:

```text
Build Your Future
Learn Web Development

[Start Learning]
```

---

## Main Content

This is where the primary information of the page is displayed.

For example:

```text
Products
Articles
Courses
Posts
Services
```

---

## Sidebar

A sidebar contains secondary information or additional navigation.

Example:

```text
Main Content        Sidebar
────────────        ───────
Article             Categories
                    Recent Posts
                    Filters
```

A sidebar is optional; not every page needs one.

---

## Footer

The footer is generally placed at the bottom of a page.

It may contain:

* Copyright information
* Contact information
* Important links
* Social media links
* Privacy policy
* Terms and conditions

Example:

```text
──────────────────────────────────
About | Contact | Privacy | Terms

© 2026 My Website
──────────────────────────────────
```

---

# 22. Page Composition Example — E-commerce

Imagine we are designing an e-commerce homepage.

```text
┌──────────────────────────────────┐
│             HEADER               │
│ Logo | Search | Account | Cart   │
├──────────────────────────────────┤
│           NAVIGATION             │
├──────────────────────────────────┤
│                                  │
│             HERO                 │
│       Big Sale — 50% OFF         │
│          [Shop Now]              │
│                                  │
├──────────────────────────────────┤
│          CATEGORIES              │
├──────────────────────────────────┤
│          PRODUCTS                │
│                                  │
│   [Card] [Card] [Card] [Card]    │
│                                  │
├──────────────────────────────────┤
│             FOOTER               │
└──────────────────────────────────┘
```

Later, HTML will be used to represent this structure.

---

# 23. HTML and Page Composition

HTML allows us to describe the structure of a page.

For example:

```html
<header>
    ...
</header>

<nav>
    ...
</nav>

<main>
    ...
</main>

<footer>
    ...
</footer>
```

This is one reason HTML is so important.

It tells the browser:

> **What each part of the page represents.**

---

# 24. Why Did HTML Need to Evolve?

The early Web was designed primarily for sharing and linking documents.

As the Web became more popular, developers wanted to build increasingly complex experiences:

```text
Simple Documents
       ↓
Images + Links
       ↓
Forms
       ↓
Multimedia
       ↓
Interactive Applications
       ↓
Modern Web Applications
```

HTML therefore evolved over time.

The modern HTML specification notes that HTML began as a language for describing documents and later adapted to applications such as purchasing systems, search systems, games, communication software, and document editing.

---

# 25. Evolution of HTML

Let's understand the major stages.

```text
Early HTML
    ↓
HTML 2.0
    ↓
HTML 3.2
    ↓
HTML 4.0 / 4.01
    ↓
XHTML
    ↓
HTML5
    ↓
HTML Living Standard
```

---

# 26. Early HTML

HTML was created as part of the early development of the Web.

Tim Berners-Lee developed the concept of the Web and created HTML as a markup language for documents.

The early Web focused heavily on:

* Documents
* Text
* Headings
* Paragraphs
* Hyperlinks

The goal was primarily:

> **Connect and share information.**

---

# 27. HTML 2.0

HTML 2.0 was an important early formal specification.

It was released in **1995**.

It provided a standardized basis for common HTML features of the time.

The early HTML history includes formal specification work by the IETF and the release of HTML 2.0 in 1995.

---

# 28. HTML 3.2

HTML 3.0 was proposed but did not become the successful standard that followed.

HTML 3.2 took a more pragmatic approach and was completed in **1997**.

It included features that had become commonly used on the Web.

---

# 29. HTML 4.0 / HTML 4.01

HTML 4 became an important milestone in the evolution of the Web.

It encouraged a clearer separation between:

```text
HTML
 ↓
Structure

CSS
 ↓
Presentation

JavaScript
 ↓
Behavior
```

This separation became an important principle of modern web development.

HTML 4.01 followed HTML 4.0 and became an ISO standard in 2000.

---

# 30. XHTML

XHTML stands for:

> **Extensible HyperText Markup Language**

XHTML was an attempt to reformulate HTML using XML syntax.

XHTML 1.0 was completed in **2000**.

The idea was to make HTML documents follow stricter XML syntax rules.

However, the Web continued to evolve based heavily on what browsers and developers were actually using.

---

# 31. WHATWG and the Modern HTML Direction

In **2004**, the **WHATWG** was formed.

WHATWG stands for:

> **Web Hypertext Application Technology Working Group**

Its goal included continuing practical development of HTML and the Web platform.

Later, WHATWG and W3C worked together on HTML5, but eventually moved toward a single continuously maintained HTML standard.

---

# 32. HTML5

HTML5 became a major milestone in modern Web Development.

The first HTML5 draft appeared in 2008, and an official HTML5 standard was published in 2014.

HTML5 introduced or standardized many capabilities important to modern web development.

Examples include semantic elements:

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

and support for technologies such as:

```text
Audio
Video
Canvas
Improved Forms
Web APIs
```

---

# 33. HTML5 Changed the Web

Before modern HTML capabilities became widely available, developers often depended more heavily on:

```text
Plugins
Flash
Non-semantic markup
```

Modern HTML provided native browser capabilities for many common use cases.

For example:

```html
<video>
    ...
</video>
```

allows browsers to work with video as part of the Web platform.

---

# 34. Is HTML5 Still the Current Version?

This is important.

Students often hear:

> "We are learning HTML5."

In modern standards terminology, HTML is now maintained as a **Living Standard** rather than being frozen into numbered versions.

The WHATWG maintains the current HTML Living Standard, and the current specification is continuously updated.

So:

```text
Old Thinking:
HTML → HTML2 → HTML3 → HTML4 → HTML5

Modern Thinking:
HTML → Living Standard
```

We can still use the term **HTML5** in learning resources because it is widely used to describe the modern era of HTML and its capabilities.

---

# 35. HTML Evolution — Timeline

```text
1990
 │
 │ Early HTML / Web
 ↓
1995
 │
 │ HTML 2.0
 ↓
1997
 │
 │ HTML 3.2
 ↓
1997–1999
 │
 │ HTML 4
 ↓
2000
 │
 │ XHTML 1.0
 ↓
2004
 │
 │ WHATWG
 ↓
2008
 │
 │ HTML5 Draft
 ↓
2014
 │
 │ HTML5 Standard
 ↓
2019
 │
 │ WHATWG + W3C move to a single HTML standard
 ↓
Today
 │
 │ HTML Living Standard
 ↓
Continuous Evolution
```

The major historical milestones above are documented by MDN and the WHATWG HTML specification.

---

# 36. Why Should We Learn HTML Today?

Because HTML is still the fundamental markup language of the Web.

It defines the structure of web documents.

For example:

```text
HTML
 ↓
Page Structure
 ↓
CSS
 ↓
Design
 ↓
JavaScript
 ↓
Behavior
```

Even modern frameworks such as React ultimately produce structures that browsers render as web documents.

---
