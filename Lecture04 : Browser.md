# 1. What is a Web Browser?

Before understanding a **Browser Engine**, let's first understand what a browser is.

A **web browser** is a software application that allows us to access and interact with resources available on the Web.

### Examples

* Google Chrome
* Mozilla Firefox
* Microsoft Edge
* Safari
* Opera

We use a browser to:

* Open websites
* Download resources
* Display web pages
* Run JavaScript
* Play media
* Store website data
* Communicate with web servers

---

# 2. What Happens When We Open a Website?

Suppose we type:

```text id="5ex3c7"
https://example.com
```

into the browser.

A simplified process looks like this:

```text id="3g0q6e"
User
 ↓
Browser
 ↓
Networking
 ↓
Server
 ↓
Response
 ↓
HTML / CSS / JS
 ↓
HTML Parsing
 ↓
DOM
 ↓
CSS Processing
 ↓
JavaScript Execution
 ↓
Rendering
 ↓
Pixels on Screen
```

This is the basic journey from:

> **Code → Browser → Pixels**

---

# 3. What is a Browser Engine?

A **browser engine** is the core part of a web browser responsible for processing web content and coordinating important browser operations.

A simplified browser architecture can be thought of as:

```text id="m9e4yv"
                 BROWSER
                    │
        ┌───────────┼───────────┐
        ↓           ↓           ↓
    Networking   Browser     Storage
                    │
              Browser Engine
                    │
          ┌─────────┴─────────┐
          ↓                   ↓
   Rendering Engine       JavaScript
                          Engine
```

The exact architecture differs between browsers, but this model is useful for beginners.

---

# 4. Browser Engines Used by Popular Browsers

Different browsers use different browser-engine technologies.

| Browser         | Browser Engine | JavaScript Engine |
| --------------- | -------------- | ----------------- |
| Google Chrome   | Blink          | V8                |
| Microsoft Edge  | Blink          | V8                |
| Mozilla Firefox | Gecko          | SpiderMonkey      |
| Apple Safari    | WebKit         | JavaScriptCore    |

> **Important:** A browser engine and a JavaScript engine are not the same thing.

---

# 5. What Does the Browser Engine Do?

When the browser receives web resources, it has to understand and process them.

For example:

```html id="j2px1e"
<h1>Hello World</h1>
```

The browser needs to understand:

```text id="z2njtl"
<h1>
 ↓
This represents a heading
```

The browser engine helps process web technologies and ultimately turn them into something that can be displayed and interacted with.

---

# 6. Major Parts We Need to Understand

For this course, think about the browser as having several important responsibilities:

```text id="9w5wzi"
Browser
│
├── Networking
│
├── HTML Parsing
│
├── DOM
│
├── CSS Processing
│
├── Rendering
│
├── JavaScript Execution
│
└── Data Persistence
```

Let's understand each one.

---

# 7. Networking

Before a browser can display a webpage, it often needs to communicate with a server.

This is handled through networking components.

### Basic Flow

```text id="3d9c3w"
Browser
   ↓
DNS
   ↓
Network Connection
   ↓
Server
   ↓
HTTP / HTTPS
   ↓
Response
```

The response may contain:

```text id="b7bqhi"
HTML
CSS
JavaScript
Images
Fonts
JSON
Videos
```

---

# 8. Example — Opening a Website

Suppose you enter:

```text id="k5f5tw"
https://example.com
```

The browser needs to:

1. Understand the URL.
2. Find the server.
3. Establish the required network connection.
4. Send an HTTP/HTTPS request.
5. Receive the response.
6. Process the returned resources.
7. Render the page.

Simplified:

```text id="gk7r89"
URL
 ↓
DNS
 ↓
Server
 ↓
HTTP Request
 ↓
HTTP Response
 ↓
Browser Processing
 ↓
Page
```

---

# 9. What is HTML Parsing?

When the browser receives HTML, it cannot simply display the raw text directly.

It first needs to **parse** the HTML.

> **Parsing means reading the HTML and understanding its structure.**

Consider:

```html id="5z4x8n"
<h1>Hello World</h1>

<p>Welcome to Web Development.</p>
```

The browser reads the markup and understands that:

```text id="v3k8y2"
<h1>
 ↓
Heading

<p>
 ↓
Paragraph
```

---

# 10. How Does HTML Parsing Work?

A simplified process is:

```text id="g1n4i0"
HTML Source
    ↓
HTML Parser
    ↓
Tokens
    ↓
DOM Tree
```

The browser reads HTML from top to bottom and constructs a structured representation of the document.

---

# 11. Example HTML

Consider:

```html id="mx3qg5"
<!DOCTYPE html>

<html>
<head>
    <title>My Page</title>
</head>

<body>

    <h1>Hello</h1>

    <p>Welcome!</p>

</body>
</html>
```

The browser doesn't think of this simply as a string.

It builds a hierarchical structure from it.

---

# 12. DOM

DOM stands for:

> **Document Object Model**

The DOM is a programming interface representing the structure of a web document as a tree of objects/nodes.

For example:

```html id="7w2y6m"
<body>
    <h1>Hello</h1>
    <p>Welcome!</p>
</body>
```

can conceptually become:

```text id="q0t4sp"
Document
   │
  html
   │
  body
  ├── h1
  │    └── "Hello"
  │
  └── p
       └── "Welcome!"
```

This is the **DOM tree**.

---

# 13. Why Do We Need the DOM?

The DOM allows JavaScript to interact with the webpage.

For example:

```javascript id="8qk1p3"
document.querySelector("h1").textContent = "Hello Students";
```

JavaScript can find the `<h1>` element and change its content.

Before:

```text id="1w4i5s"
Hello
```

After JavaScript:

```text id="5i8o7r"
Hello Students
```

The page can therefore change without replacing the entire document.

---

# 14. DOM as a Tree

Let's take this HTML:

```html id="m5p3nb"
<div>
    <h1>Web Development</h1>
    <p>Learn HTML.</p>
</div>
```

The DOM can be visualized as:

```text id="6azk7p"
Document
   │
   └── div
       ├── h1
       │   └── "Web Development"
       │
       └── p
           └── "Learn HTML."
```

Every element can be represented as a node in the tree.

---

# 15. Parent and Child Relationships

The DOM has relationships between nodes.

For example:

```text id="2a5f8w"
div
├── h1
└── p
```

Here:

```text id="x4p2m1"
div
 ↓
Parent

h1
 ↓
Child

p
 ↓
Child
```

This parent-child relationship becomes extremely important when we start working with JavaScript and DOM manipulation.

---

# 16. HTML Parsing vs DOM

These are related but not exactly the same.

### HTML Parsing

The browser reads HTML source and interprets its markup.

```text id="5khj6q"
HTML
 ↓
Parser
```

### DOM

The browser builds a structured representation of the document.

```text id="xy7p9k"
Parsed HTML
 ↓
DOM Tree
```

So:

```text id="v8n5c2"
HTML
 ↓
HTML Parser
 ↓
DOM
```

---

# 17. What is a JavaScript Engine?

A **JavaScript engine** is the component that executes JavaScript code.

# 18. JavaScript Engines in Popular Browsers

| Browser | JavaScript Engine |
| ------- | ----------------- |
| Chrome  | V8                |
| Edge    | V8                |
| Firefox | SpiderMonkey      |
| Safari  | JavaScriptCore    |

### Important

Do not confuse:

```text id="4r8a9x"
Browser Engine
       ≠
JavaScript Engine
```

For example:

```text id="04e4zv"
Chrome
│
├── Blink
│    ↓
│  Browser / Rendering Engine
│
└── V8
     ↓
   JavaScript Engine
```

---

# 19. What Does a JavaScript Engine Do?

When the user clicks the button:

```text id="k1x2r6"
Click
 ↓
JavaScript
 ↓
JavaScript Engine
 ↓
DOM API
 ↓
DOM Changes
 ↓
Browser Updates Page
```

This is how JavaScript can make webpages interactive.

---

# 20. Rendering Engine

Now we have:

```text id="v8j3g1"
HTML → DOM
JavaScript → JS Engine
```

But how does the browser actually show the page on the screen?

This is where **rendering** comes in.

A rendering engine processes the document and styling information to determine what should appear on the screen.

---

# 21. What is Rendering?

**Rendering** is the process of converting processed web content into the visual output that appears on the screen.

Simplified:

```text id="e1f4s7"
HTML
 ↓
DOM
 ↓
CSS
 ↓
Layout
 ↓
Painting
 ↓
Pixels
 ↓
Screen
```

---

# 22. HTML + CSS Example

Suppose we have:

```html id="0e7l5m"
<h1>Hello World</h1>
```

and CSS:

```css id="r2h5g8"
h1 {
    color: blue;
    font-size: 40px;
}
```

The browser needs to determine:

* What element exists?
* What styles apply?
* Where should it appear?
* How large should it be?
* How should it be painted?

Then the result appears on the screen.

---

# 23. Simplified Rendering Pipeline

A simplified model is:

```text id="x6z0f5"
HTML
 ↓
DOM
 ↓
CSS
 ↓
Style Calculation
 ↓
Layout
 ↓
Paint
 ↓
Composite
 ↓
Screen
```

### Style Calculation

The browser determines which CSS rules apply.

### Layout

The browser calculates:

* Position
* Width
* Height
* Spacing

### Paint

The browser draws visual elements such as:

* Text
* Colors
* Borders
* Images
* Shadows

### Composite

The browser combines visual layers for final display.

> The exact browser pipeline is more complex and can differ depending on the browser and situation. This simplified model is intended for understanding the basic idea.

---

# 24. Networking Inside the Browser

The browser needs networking to retrieve resources.

For example:

```text id="v8b8f6"
HTML
 ↓
CSS
 ↓
JavaScript
 ↓
Images
 ↓
Fonts
```

These resources may come from:

* The same server
* A CDN
* Another server
* An API

The browser manages the network communication needed to retrieve them.

---

# 25. Example — Loading a Website

Suppose `index.html` contains:

```html id="wq6n8r"
<link rel="stylesheet" href="style.css">

<script src="script.js"></script>

<img src="logo.png">
```

The browser may need to retrieve:

```text id="p2k5m7"
index.html
     ↓
 ┌───┼────────┐
 ↓   ↓        ↓
CSS JS       Image
```

The networking layer handles the requests needed to obtain these resources.

---

# 26. Data Persistence

Now imagine you visit a website.

The browser may need to remember certain information between page loads or visits.

This concept is called:

> **Data Persistence**

Persistence means:

> **Data continues to exist after the current page or session ends, depending on the storage mechanism.**

---

# 27. Why Does a Browser Store Data?

Websites may need to store information such as:

* Preferences
* Login/session-related information
* Shopping cart information
* Application settings
* Cached resources
* Other website data

Browsers provide different storage mechanisms for different purposes.

---

> **Next Lecture → HTML: Document Structure, Tags, Elements & Attributes**
