# 🌐 HTML — HyperText Markup Language

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Markup%20Language-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5 Badge">
  <img src="https://img.shields.io/badge/Level-Beginner-22C55E?style=for-the-badge" alt="Beginner Level">
  <img src="https://img.shields.io/badge/Status-Learning-0EA5E9?style=for-the-badge" alt="Learning Status">
</p>

<p align="center">
  <b>My Web Development Notes</b>
  <br>
  A beginner-friendly guide to HTML fundamentals, document structure, elements, web browsers, and the evolution of HTML.
</p>

---

## 📑 Table of Contents

- [📌 What Is HTML?](#-what-is-html)
- [🏗️ Basic HTML Document Structure](#️-basic-html-document-structure)
- [🧩 Understanding HTML Tags](#-understanding-html-tags)
- [📄 HTML Elements](#-html-elements)
- [🧠 Understanding the Head Section](#-understanding-the-head-section)
- [🌍 What Is a Web Browser?](#-what-is-a-web-browser)
- [📜 History of HTML](#-history-of-html)
- [🎯 Key Takeaways](#-key-takeaways)
- [🚀 What's Next?](#-whats-next)

---

## 📌 What Is HTML?

**HTML stands for HyperText Markup Language.** It is the standard markup language used to create and structure web pages. HTML provides the basic structure of a website by defining elements such as headings, paragraphs, images, links, lists, tables, forms, and other content.

HTML uses a collection of elements and tags to describe the meaning and organization of content. A web browser interprets this structure and displays the resulting page to the user.

Despite being used to build websites, **HTML is a markup language, not a programming language**, because it does not provide general-purpose programming logic such as loops and conditional statements.

### 💡 Why Is HTML Important?

- 🏗️ **Structure:** Defines the layout and organization of web page content.
- 📝 **Content:** Adds headings, paragraphs, images, links, and lists.
- ♿ **Accessibility:** Provides semantic information that helps assistive technologies understand content.
- 🔍 **SEO:** Helps search engines understand the meaning and structure of a page.
- 🎨 **Works with CSS:** CSS controls the visual appearance of HTML content.
- ⚡ **Works with JavaScript:** JavaScript adds interactivity and dynamic behavior.

### 🛠️ Core Web Technologies

| Technology | Main Purpose |
|---|---|
| HTML | Structures web content |
| CSS | Styles and designs web pages |
| JavaScript | Adds logic and interactivity |

---

## 🏗️ Basic HTML Document Structure

Every standard HTML document begins with a document type declaration, followed by the root HTML element. Inside it, the document is divided into the head and body sections.

### 💻 Example: Basic HTML5 Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Web Page</title>
</head>
<body>

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

</body>
</html>
```

### 🔍 Explanation of Each Tag

| Tag or Declaration | Meaning |
|---|---|
| `<!DOCTYPE html>` | Declares the document as HTML5 and enables standards mode in browsers. |
| `<html>` | The root element containing the entire HTML document. |
| `<head>` | Contains metadata and resources used by the browser. |
| `<meta>` | Provides metadata, such as character encoding and viewport settings. |
| `<title>` | Defines the page title shown in the browser tab. |
| `<body>` | Contains the page content displayed in the browser. |
| `<h1>` | Defines a top-level heading. |
| `<p>` | Defines a paragraph. |

### 1. `<!DOCTYPE html>`

The DOCTYPE declaration tells the browser to interpret the document using modern HTML standards. It is not an HTML element and does not require a closing tag.

### 2. `<html>`

The `<html>` element is the root element of the document. It contains the `<head>` and `<body>` sections. The `lang="en"` attribute identifies English as the primary language of the page.

### 3. `<head>`

The `<head>` element contains metadata about the document, along with information and resources that help the browser process the page. Most of its contents are not displayed directly within the page itself.

### 4. `<title>`

The `<title>` element specifies the document's title, which normally appears in the browser tab and can also be used by bookmarks and search engines.

### 5. `<body>`

The `<body>` element contains the main content of the webpage, including headings, paragraphs, images, links, tables, and forms. This is where most visible page content is written.

---

## 🧠 Understanding the Head Section

**Metadata means data about data.** In HTML, metadata provides information about the webpage itself rather than being the main content displayed to the user.

Metadata can describe the document's character encoding, page title, viewport behavior, description, author, and other properties.

### Example of HTML Metadata

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Beginner-friendly HTML notes.">
    <title>HTML Learning Notes</title>
</head>
```

**Common metadata elements:**

- `charset="UTF-8"` — specifies character encoding so that a wide range of characters can be represented correctly.
- `name="viewport"` — helps the webpage adapt to different screen sizes, including mobile devices.
- `name="description"` — provides a short description of the page that search engines may use in search results.
- `<title>` — sets the document title shown in the browser tab.

---

## 🧩 Understanding HTML Tags

HTML tags are written inside angle brackets (`<` and `>`). Most HTML elements use an opening tag and a closing tag to surround their content.

### Syntax

```html
<tagname>Content goes here...</tagname>
```

### Examples

```html
<h1>My First Heading</h1>
<p>My first paragraph.</p>
```

In the first example, `<h1>` is the opening tag, `My First Heading` is the content, and `</h1>` is the closing tag.

The forward slash (`/`) in the closing tag indicates the end of the element.

---

## 📄 HTML Elements

An **HTML element** generally consists of an opening tag, its content, and a closing tag. Some elements, however, are empty and do not have closing tags.

### General Syntax

```html
<tagname>Content goes here...</tagname>
```

### Example

```html
<h1>Welcome to HTML</h1>
<p>HTML is used to structure web pages.</p>
```

### Empty HTML Elements

Some HTML elements do not contain content between opening and closing tags. These are commonly called **void elements**.

Examples include:

```html
<br>
<hr>
<img src="image.jpg" alt="A sample image">
<input type="text">
```

- `<br>` — inserts a line break.
- `<hr>` — represents a thematic break, commonly displayed as a horizontal line.
- `<img>` — embeds an image.
- `<input>` — creates an input control for forms.

**Important note:** Void elements must not have closing tags. For example, write `<br>`, not `</br>`. In HTML, the trailing slash in `<br />` is optional and does not change its meaning.

---

## 🌍 What Is a Web Browser?

A **web browser** is a software application that retrieves, interprets, and displays web content. Examples include Google Chrome, Microsoft Edge, Mozilla Firefox, Safari, and Opera.

The main role of a browser when handling HTML is to parse the document, build its internal representation, and render the content on the screen.

A browser does not normally display HTML tags as literal text. Instead, it uses those tags and their attributes to determine the structure and meaning of the page.

### How a Browser Displays an HTML Page

1. The browser retrieves or opens the HTML document.
2. It parses the HTML markup.
3. It constructs a Document Object Model (DOM) representing the document structure.
4. It processes CSS and other resources when available.
5. It renders the page for the user.

### Example

HTML source:

```html
<h1>Hello World</h1>
<p>Welcome to my website.</p>
```

Browser output:

# Hello World

Welcome to my website.

The browser displays the heading and paragraph rather than showing the tags themselves.

---

## 📜 History of HTML

HTML has evolved over time to support richer, more accessible, and more interactive websites.

| Year | Milestone |
|---|---|
| 1989 | Tim Berners-Lee proposed the World Wide Web. |
| 1991 | Tim Berners-Lee described the early version of HTML. |
| 1993 | Dave Raggett circulated the HTML+ proposal. |
| 1995 | HTML 2.0 was published as an early formal specification. |
| 1997 | HTML 3.2 became a W3C Recommendation. |
| 1999 | HTML 4.01 became a W3C Recommendation. |
| 2000 | XHTML 1.0 became a W3C Recommendation. |
| 2008 | The WHATWG HTML5 specification was published as a public draft. |
| 2012 | The WHATWG continued developing HTML as a Living Standard. |
| 2014 | HTML5 became a W3C Recommendation. |
| 2016 | HTML 5.1 reached W3C Candidate Recommendation status. |
| 2017 | HTML 5.1 Second Edition and HTML 5.2 became W3C Recommendations. |

**Note:** HTML development continues. The WHATWG HTML Living Standard is maintained and updated over time, rather than being limited to numbered versions alone.

---

## 🎯 Key Takeaways

- HTML stands for **HyperText Markup Language**.
- HTML is a markup language, not a programming language.
- `<!DOCTYPE html>` declares the document type and enables standards mode.
- The `<html>` element is the root of the document.
- The `<head>` section contains metadata and resource references.
- The `<title>` element defines the document title.
- The `<body>` section contains the webpage's main content.
- Most HTML elements have opening and closing tags.
- Void elements, such as `<br>` and `<img>`, do not have closing tags.
- Web browsers parse HTML and render its content for users.
- HTML provides structure, CSS provides styling, and JavaScript provides interactivity.

---
<p align="center">
  <b>Keep Learning. Keep Building. Keep Improving. 🚀</b>
  <br>
  <sub>Part of my Web Development Notes — created and maintained as I learn.</sub>
</p>
