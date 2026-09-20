# Types of HTML Elements

HTML elements can be broadly understood by looking at **how they contain content** and **how they behave**.

For beginners, we can understand them in four categories:

1. **Normal Elements**
2. **Void Elements**
3. **Raw Text Elements**
4. **RCDATA Elements**
5. **Foreign Elements**

Let's understand each one with simple examples.

---

# 1. Normal Elements

Normal elements have:

* An opening tag
* Content
* A closing tag

### Basic Structure

```html
<opening-tag>
    Content
</closing-tag>
```

### Example

```html
<h1>Hello World</h1>
```

Here:

```html
<h1>
```

is the opening tag.

```text
Hello World
```

is the content.

```html
</h1>
```

is the closing tag.

So:

```text
Opening Tag + Content + Closing Tag
              ↓
          HTML Element
```

### More Examples

```html
<p>This is a paragraph.</p>

<h1>My Website</h1>

<div>This is a container.</div>

<button>Click Me</button>
```

All of these have an opening tag and a closing tag.

### Output

```text
My Website

This is a paragraph.

This is a container.

[Click Me]
```

### Simple Rule

> **Normal Element = Opening Tag + Content + Closing Tag**

---

# 2. Void Elements

A **void element** does not have a closing tag.

It is used when an element does not need to contain content.

### Example

```html
<br>
```

`<br>` is used to create a line break.

Example:

```html
<p>Hello<br>World</p>
```

### Output

```text
Hello
World
```

Notice that we don't write:

```html
</br>
```

We simply write:

```html
<br>
```

---

## Another Example — `<img>`

```html
<img src="photo.jpg" alt="My Photo">
```

An image element doesn't contain text between an opening and closing tag.

### Output

If `photo.jpg` exists:

```text
[Image appears here]
```

---

## Common Void Elements

Some commonly encountered void elements are:

```html
<br>
<hr>
<img>
<input>
<meta>
<link>
```

For example:

```html
<input type="text">
```

### Output

```text
[________________]
```

It creates an input field.

### Important

Don't write:

```html
<input></input>
```

For HTML void elements, there is no separate closing tag.

### Simple Rule

> **Void Element = No Closing Tag**

---

# 3. Raw Text Elements

Now we come to **Raw Text Elements**.

This sounds complicated, but the basic idea is simple.

A raw text element contains text that the browser should treat as **raw text rather than normal HTML markup**.

The main examples are:

```html
<script>
```

and:

```html
<style>
```

For example:

```html
<script>
    alert("Hello");
</script>
```

Inside `<script>`, the browser treats the content as JavaScript code.

It does not treat:

```javascript
alert("Hello");
```

as normal HTML text.

---

## Example

```html
<script>
    console.log("Hello World");
</script>
```

Here:

```html
<script>
```

starts the script section.

```html
</script>
```

ends the script section.

Everything inside is treated as JavaScript source code.

---

## Another Example — `<style>`

```html
<style>
    body {
        background: black;
    }
</style>
```

The content inside `<style>` is treated as CSS.

So:

```text
<script> → JavaScript
<style>  → CSS
```

### Important

We are **not learning JavaScript or CSS here**.

The important thing to understand is only:

> Raw text elements contain content that is treated as raw text/code rather than being parsed as normal HTML markup.

### Simple Rule

> **Raw Text Element = Content is treated as raw text/code**

---

# 4. RCDATA Elements

RCDATA stands for:

> **Replaceable Character Data**

The name sounds complicated, but the basic idea is simple.

RCDATA elements allow text content where **HTML tags are generally treated as text**, while character references can still be interpreted.

The main HTML examples are:

```html
<textarea>
```

and:

```html
<title>
```

---

## Example with `<textarea>`

```html
<textarea>
<h1>Hello World</h1>
</textarea>
```

The important thing is that:

```html
<h1>Hello World</h1>
```

inside the `<textarea>` is treated as text entered into the textarea, rather than creating an actual heading.

### Output

```text
┌──────────────────────────────┐
│ <h1>Hello World</h1>         │
│                              │
└──────────────────────────────┘
```

The browser does **not** create an `<h1>` heading there.

It displays the characters as text inside the textarea.

---

## Example with `<title>`

```html
<title>
    My Website
</title>
```

The text:

```text
My Website
```

is treated as the title text of the document.

The browser does not display it as normal webpage content inside `<body>`.

Instead, it can appear in the browser tab.

### Simple Rule

> **RCDATA = Text content where HTML markup is generally not interpreted as normal HTML elements.**

For beginners, remember the two important examples:

```text
<title>
<textarea>
```

---

# 5. Foreign Elements

Foreign elements are elements that come from **other markup vocabularies** that can be embedded inside an HTML document.

The two important examples for beginners are:

```text
SVG
MathML
```

---

## SVG Example

SVG stands for:

> **Scalable Vector Graphics**

HTML allows us to use SVG inside a webpage.

For example:

```html
<svg width="100" height="100">
    <circle cx="50" cy="50" r="40"></circle>
</svg>
```

This creates a simple circle.

### Output

```text
        ●
```

The important point is that:

```html
<svg>
```

belongs to the SVG markup vocabulary rather than being an ordinary HTML element.

---

## MathML Example

HTML can also contain MathML for mathematical notation.

For example:

```html
<math>
    <mi>x</mi>
    <mo>+</mo>
    <mi>y</mi>
</math>
```

This represents mathematical content.

So the basic idea is:

```text
HTML Document
     │
     ├── HTML Elements
     │
     ├── SVG Elements
     │
     └── MathML Elements
```

### Simple Rule

> **Foreign Elements = Elements from another markup vocabulary, such as SVG or MathML, used inside HTML.**

---
