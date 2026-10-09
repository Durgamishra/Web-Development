# 📘 HTML Fundamentals — Headings, Paragraphs, Links & Images

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Fundamentals-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Level-Beginner-22C55E?style=for-the-badge" alt="Beginner">
</p>

## 📑 Table of Contents

- [1. HTML Headings](#-1-html-headings)
- [2. HTML Paragraphs](#-2-html-paragraphs)
- [3. HTML Links](#-3-html-links)
- [4. HTML Images](#-4-html-images)
- [5. Quick Revision](#-5-quick-revision)

---

## 🏷️ 1. HTML Headings

HTML provides **six heading elements**, ranging from `<h1>` to `<h6>`. These elements define headings and subheadings within a webpage. `<h1>` represents the highest-level heading, while `<h6>` represents the lowest-level heading.

### 💻 Syntax

```html
<h1>This is Heading 1</h1>
<h2>This is Heading 2</h2>
<h3>This is Heading 3</h3>
<h4>This is Heading 4</h4>
<h5>This is Heading 5</h5>
<h6>This is Heading 6</h6>
```

### 📖 Explanation

| Tag | Meaning | Typical Use |
|---|---|---|
| `<h1>` | Heading 1 | Main page heading |
| `<h2>` | Heading 2 | Major section heading |
| `<h3>` | Heading 3 | Subsection heading |
| `<h4>` | Heading 4 | Smaller subsection |
| `<h5>` | Heading 5 | Lower-level heading |
| `<h6>` | Heading 6 | Lowest-level heading |

### 🧠 Important Points

- HTML contains six heading elements: `<h1>` through `<h6>`.
- Browsers usually display headings in bold, with `<h1>` larger than `<h6>` by default.
- Headings help organize content into a meaningful hierarchy.
- Use headings according to their meaning and structure, not merely to change text size.
- CSS can be used to customize the appearance of any heading.

**Example:**

```html
<h1>Web Development</h1>

<h2>HTML</h2>
<p>HTML provides structure to webpages.</p>

<h2>CSS</h2>
<p>CSS controls the appearance of webpages.</p>

<h3>CSS Colors</h3>
<p>Colors help improve the visual design.</p>
```

---

## 📝 2. HTML Paragraphs

The HTML `<p>` element is used to define a paragraph of text. It allows you to organize written content into separate blocks, making a webpage easier to read and understand.

### 💻 Syntax

```html
<p>This is a paragraph.</p>

<p>This is another paragraph.</p>
```

### 📖 Explanation

- `<p>` is the opening tag.
- `This is a paragraph.` is the content.
- `</p>` is the closing tag.

Browsers normally display each paragraph as a separate block, with some space before or after it.

### 💡 Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>HTML Paragraphs</title>
</head>
<body>

    <h1>About HTML</h1>

    <p>HTML stands for HyperText Markup Language.</p>

    <p>It is used to structure content on webpages.</p>

</body>
</html>
```

### 🧠 Important Points

- Every paragraph generally begins with `<p>` and ends with `</p>`.
- Browsers automatically add spacing around paragraphs.
- Extra spaces and line breaks in the HTML source are generally collapsed when rendered.
- Use `<br>` when a line break is specifically needed within content.
- Use CSS to control paragraph spacing, alignment, font size, and line height.

---

## 🔗 3. HTML Links

The HTML `<a>` element, also known as the **anchor element**, is used to create hyperlinks. A hyperlink allows users to navigate to another webpage, a file, a section of the current page, or another supported destination.

### 💻 Syntax

```html
<a href="https://www.google.com">Visit Google</a>
```

### 📖 What Does `href` Mean?

**`href` stands for Hypertext Reference.**

It is an HTML attribute used inside the `<a>` element to specify the destination URL or location of a hyperlink.

In the example above:

- `<a>` defines the anchor element.
- `href` specifies the destination.
- `https://www.google.com` is the destination URL.
- `Visit Google` is the clickable text.
- `</a>` closes the anchor element.

**Important:** Use the complete URL, including `https://`, for an external website. Writing `www.google.com` without a scheme may cause the browser to interpret it as a relative URL instead of the intended external destination.

### 💻 More Examples

**1. Link to an external website**

```html
<a href="https://www.google.com">Google</a>
```

**2. Link to another page in your project**

```html
<a href="about.html">About Us</a>
```

**3. Open a link in a new tab**

```html
<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">
    Open Google
</a>
```

**4. Link to a section on the same page**

```html
<a href="#contact">Go to Contact</a>

<h2 id="contact">Contact Us</h2>
```

### 🧠 Important Points

- Links are created using the `<a>` element.
- `href` means Hypertext Reference.
- The destination can be an external URL, a local file, or a section identifier.
- The clickable content can be text or an image.
- Use meaningful link text so users understand where the link will take them.

---

## 🖼️ 4. HTML Images

The HTML `<img>` element is used to display an image on a webpage. It is a **void element**, which means it does not require a closing tag.

### 💻 Syntax

```html
<img src="image.jpg" alt="A sample image" width="104" height="142">
```

### 📖 Explanation of Attributes

| Attribute | Meaning | Purpose |
|---|---|---|
| `src` | Source | Specifies the path or URL of the image. |
| `alt` | Alternative text | Describes the image if it cannot load and supports screen readers. |
| `width` | Width | Specifies the image width, normally in CSS pixels when written as a number in HTML. |
| `height` | Height | Specifies the image height, normally in CSS pixels when written as a number in HTML. |

### 💡 Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>HTML Images</title>
</head>
<body>

    <h1>My Image</h1>

    <img
        src="image.jpg"
        alt="A beautiful landscape"
        width="300"
        height="200"
    >

</body>
</html>
```

### 📂 Understanding the `src` Attribute

The `src` attribute tells the browser where the image file is located.

For example:

```html
<img src="image.jpg" alt="Sample image">
```

This expects `image.jpg` to be available at the relative path resolved from the current page's URL.

If the image is stored inside an `images` folder, write:

```html
<img src="images/image.jpg" alt="Sample image">
```

### 🧠 Important Points

- `<img>` embeds an image into a webpage.
- `src` specifies the image location.
- `alt` provides a text alternative for accessibility.
- `width` and `height` control the image's displayed dimensions.
- The `<img>` element does not need a closing tag.
- Always provide appropriate alternative text for meaningful images. For purely decorative images, use `alt=""`.

---

## ⚡ 5. Quick Revision

| HTML Element or Attribute | Definition |
|---|---|
| `<h1>`–`<h6>` | Defines six levels of headings. |
| `<p>` | Defines a paragraph. |
| `<a>` | Creates a hyperlink. |
| `href` | Hypertext Reference; specifies a link destination. |
| `<img>` | Embeds an image. |
| `src` | Specifies the source or location of an image. |
| `alt` | Provides alternative text for an image. |
| `width` | Specifies the image's width. |
| `height` | Specifies the image's height. |
| `target="_blank"` | Requests that a link open in a new browsing context, usually a new tab. |

### 🎯 Practice Exercise

Create an HTML page that includes:

- [ ] One main heading using `<h1>`.
- [ ] Two subheadings using `<h2>`.
- [ ] Two paragraphs using `<p>`.
- [ ] A hyperlink to Google using `href`.
- [ ] An image using `src`, `alt`, `width`, and `height`.

---

<p align="center">
  <b>🚀 Learn the fundamentals. Practice the code. Build the web.</b>
  <br>
  <sub>Web Development Notes | HTML Basics</sub>
</p>