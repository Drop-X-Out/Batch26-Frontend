# HTML Basics

## 1. What is HTML?

**HTML stands for HyperText Markup Language.**

HTML is a **standard markup language used to create and structure web pages.**

# 2. HTML Full Form

```text
HTML
│
├── H → Hyper
├── T → Text
├── M → Markup
└── L → Language
```

So:

> **HTML = HyperText Markup Language**

Now let's understand each word separately.

---

# 3. What is Hyper?

**Hyper** means something that goes beyond or connects to something else.

In HTML, we commonly see the idea of **HyperText**.

For example, suppose you see this on a webpage:

```text
Visit Google
```

If you click **Visit Google**, you can go to another webpage.

This connection between one piece of text and another webpage is the basic idea behind **HyperText**.

---

# 4. What is Text?

Text simply means written information.

For example:

```text
Welcome to my website
```

This is text.

# 5. What is HyperText?

Now combine:

```text
Hyper + Text
```

We get:

> **HyperText**

HyperText means text that can be connected to another document or webpage, commonly through a link.

Here:

```text
Visit Google
```

is clickable text.

When the user clicks it, the browser can navigate to Google.

### Output

**Visit Google**

The important idea is:

```text
Text
  ↓
Clickable
  ↓
Another webpage
```

This is the basic idea of **HyperText**.

---

# 6. What is Markup?

Now let's understand the word:

> **Markup**

Markup means adding **special tags/labels around content to describe its structure or meaning.**

For example:

```html
<h1>Welcome to My Website</h1>
```

Here:

```html
<h1>
```

tells the browser:

> This is a heading.

And:

```html
</h1>
```

tells the browser:

> The heading ends here.

So HTML is adding markup to the content.

### Simple Example

Without markup:

```text
Welcome to My Website
```

With HTML markup:

```html
<h1>Welcome to My Website</h1>
```

Now the browser understands that:

> **"Welcome to My Website" is a heading.**

---

# 8. What is Language?

A **language** is a system of rules and symbols used to communicate information.

For example:

* English is a language.
* Hindi is a language.
* JavaScript is a programming language.
* HTML is a markup language.

HTML has its own:

* Tags
* Elements
* Attributes
* Rules
* Syntax

For example:

```html
<h1>Hello World</h1>
```

This follows the rules of HTML.

Therefore, HTML is called a **Markup Language**.

---

# 9. What is a Markup Language?

Now combine:

```text
Markup + Language
```

A **markup language** is a language that uses markup to describe the structure and meaning of content.

HTML uses tags to describe webpage content.

For example:

```html
<h1>My Website</h1>

<p>Welcome to my website.</p>
```

Here:

```html
<h1>
```

marks the content as a heading.

And:

```html
<p>
```

marks the content as a paragraph.

So:

> **HTML is a markup language because it uses markup/tags to describe the structure of webpage content.**

---

# 10. Is HTML a Programming Language?

**No. HTML is not a programming language.**

HTML is a **markup language**.

A programming language is used to write instructions that can perform logic and operations.

Programming languages can work with concepts such as:

* Variables
* Conditions
* Loops
* Functions
* Calculations
* Logic

For example, JavaScript can perform a calculation:

HTML mainly describes the structure of content:

```html
<h1>Hello World</h1>
```

It tells the browser:

> "This is a heading."

It is not performing a programming operation.

---

# 12. Let's Write Our First HTML Program

Now let's create our **first HTML program**.

Create a file:

```text
index.html
```

Write the following code:

```html
<!DOCTYPE html>

<html>

<head>
    <title>My First Web Page</title>
</head>

<body>

    <h1>Hello World</h1>

</body>

</html>
```

This is the **basic structure of an HTML document**.

---

# 13. Output

When we open this file in the browser, the output will be:

# Hello World

And the browser tab will show:

```text
My First Web Page
```

---

# 14. Understanding the Basic HTML Structure

Our complete structure is:

```text
<!DOCTYPE html>

<html>

    <head>
        <title>My First Web Page</title>
    </head>

    <body>
        <h1>Hello World</h1>
    </body>

</html>
```

The basic structure can be visualized as:

```text
HTML Document
│
├── HEAD
│   └── TITLE
│
└── BODY
    └── H1
```

Now let's understand it **line by line**.

---

# 15. Line 1 — `<!DOCTYPE html>`

```html
<!DOCTYPE html>
```

This is called the **DOCTYPE declaration**.

It tells the browser:

> This document is an HTML document and should be interpreted using the modern HTML standard.

It is written at the beginning of the HTML document.

### Important

`<!DOCTYPE html>` is a **declaration**, not a normal HTML element.

---

# 16. Line 2 — `<html>`

```html
<html>
```

This is the **root element** of the HTML document.

It tells the browser:

> The HTML document starts here.

Everything in our HTML document is generally placed inside:

```html
<html>

    ...

</html>
```

So `<html>` is the outermost element.

---

# 17. `<head>`

Inside `<html>`, we have:

```html
<head>
    
</head>
```

The `<head>` contains information **about the webpage/document**.

For example, it can contain:

* Page title
* Metadata
* CSS links
* Other document information

For now, we are only using:

```html
<title>My First Web Page</title>
```

---

# 18. `<title>`

```html
<title>My First Web Page</title>
```

The `<title>` defines the title of the HTML document.

You can normally see it in the **browser tab**.

For example:

```text
┌──────────────────────────────┐
│ My First Web Page       ×    │
└──────────────────────────────┘
```

The title is:

```text
My First Web Page
```

It is not normally displayed as the main content inside the webpage.

---

# 19. `<body>`

Next we have:

```html
<body>

</body>
```

The `<body>` contains the main content of the webpage.

For example:

```html
<body>

    <h1>Hello World</h1>

</body>
```

The content inside the body is what the user normally sees on the webpage.

---

# 20. `<h1>`

Inside the body we have:

```html
<h1>Hello World</h1>
```

`<h1>` represents a heading.

The content is:

```text
Hello World
```

The opening tag is:

```html
<h1>
```

The closing tag is:

```html
</h1>
```

Together:

```html
<h1>Hello World</h1>
```

form an HTML element.

---

# 21. Opening Tag and Closing Tag

Look at:

```html
<h1>Hello World</h1>
```

Break it down:

```text
<h1>
 ↓
Opening Tag

Hello World
 ↓
Content

</h1>
 ↓
Closing Tag
```

So:

```text
Opening Tag + Content + Closing Tag
             ↓
          Element
```

---

# 22. Complete Structure

Now let's look at the complete document again:

```html
<!DOCTYPE html>

<html>

<head>
    <title>My First Web Page</title>
</head>

<body>
    <h1>Hello World</h1>
</body>

</html>
```

Think of it like this:

```text
<!DOCTYPE html>
       │
       ↓
     <html>
       │
       ├───────────────┐
       ↓               ↓
    <head>           <body>
       │               │
       ↓               ↓
    <title>           <h1>
```

---
# 24. One More Very Small Program

Now let's add a paragraph.

```html
<!DOCTYPE html>

<html>

<head>
    <title>My First Web Page</title>
</head>

<body>

    <h1>Hello World</h1>

    <p>Welcome to my first webpage.</p>

</body>

</html>
```

### Output

# Hello World

Welcome to my first webpage.
