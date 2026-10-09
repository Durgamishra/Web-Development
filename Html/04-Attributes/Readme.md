# ⚙️ HTML Attributes

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Attributes-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Topic-Web%20Development-0EA5E9?style=for-the-badge" alt="Web Development">
  <img src="https://img.shields.io/badge/Level-Beginner-22C55E?style=for-the-badge" alt="Beginner">
</p>

**HTML attributes** provide additional information about HTML elements. They are written inside the opening tag and usually consist of a name and a value. Attributes help define the behavior, appearance, destination, language, and other properties of an element.

## 📑 Table of Contents

- [1. Syntax of HTML Attributes](#-1-syntax-of-html-attributes)
- [2. The `href` Attribute](#-2-the-href-attribute)
- [3. Absolute and Relative URLs](#-3-absolute-and-relative-urls)
- [4. The `src` Attribute](#-4-the-src-attribute)
- [5. The `width` and `height` Attributes](#️-5-the-width-and-height-attributes)
- [6. The `alt` Attribute](#️-6-the-alt-attribute)
- [7. The `style` Attribute](#-7-the-style-attribute)
- [8. The `lang` Attribute](#-8-the-lang-attribute)
- [9. The `title` Attribute](#️-9-the-title-attribute)
- [10. Important Rules](#-10-important-rules)
- [11. Quick Summary](#-11-quick-summary)

---

## 🧩 1. Syntax of HTML Attributes

Attributes are written inside the opening tag of an HTML element. The general syntax is:

```html
<tagname attribute_name="attribute_value">Content</tagname>
```

### Example

```html
<a href="https://www.w3schools.com">Visit W3Schools</a>
```

In this example:

- `<a>` is the anchor element.
- `href` is the attribute name.
- `"https://www.w3schools.com"` is the attribute value.
- `Visit W3Schools` is the clickable link text.

**Important:** Attributes are written inside the opening tag, not the closing tag.

---

## 🔗 2. The `href` Attribute

The `href` attribute stands for **Hypertext Reference**. It specifies the destination of a hyperlink created using the `<a>` element.

### Example

```html
<a href="https://www.w3schools.com">Visit W3Schools</a>
```

When a user clicks the text `Visit W3Schools`, the browser navigates to the specified website.

### Another Example

```html
<a href="about.html">About Us</a>
```

This link points to a local page named `about.html`, relative to the current document's URL.

---

## 🌐 3. Absolute and Relative URLs

URLs used in HTML can be absolute or relative. They are commonly used in attributes such as `href` and `src`.

### A. Absolute URL

An **absolute URL** specifies the complete address of a resource, usually including the protocol and domain name.

Example:

```html
<a href="https://www.w3schools.com">Visit W3Schools</a>

<img
    src="https://www.w3schools.com/images/img_girl.jpg"
    alt="A girl wearing a jacket"
>
```

**Explanation:** The browser uses the complete URL to locate the external webpage or image. The resource must be available at that address.

### B. Relative URL

A **relative URL** specifies a resource's location relative to the current document's URL or base URL.

Suppose your project has the following structure:

```text
my-website/
├── index.html
├── about.html
└── images/
    └── girl.jpg
```

You can use these relative URLs:

```html
<a href="about.html">About Us</a>

<img src="images/girl.jpg" alt="A girl wearing a jacket">
```

**Explanation:** The browser resolves `about.html` and `images/girl.jpg` relative to the current page's location.

### Comparison

| Absolute URL | Relative URL |
|---|---|
| Specifies a complete resource address. | Specifies a path relative to a base URL. |
| Commonly includes the protocol and domain. | Usually omits the protocol and domain. |
| Example: `https://example.com/image.jpg` | Example: `images/image.jpg` |
| Useful for linking to external resources. | Useful for linking to files within a website. |

**Note:** Absolute URLs can also point to resources on your own website. Relative URLs are not limited to local computer files; they are commonly used on deployed websites too.

---

## 🖼️ 4. The `src` Attribute

The `src` attribute stands for **Source**. It specifies the location of a resource that an HTML element should load. It is commonly used with the `<img>` element to display images.

### Example: External Image

```html
<img
    src="https://www.w3schools.com/images/img_girl.jpg"
    alt="A girl wearing a jacket"
>
```

### Example: Local Image

```html
<img src="images/girl.jpg" alt="A girl wearing a jacket">
```

**Explanation:**

- `src` tells the browser where to find the image.
- The browser attempts to load the image from that location.
- If the path is incorrect or the image is unavailable, the image may not appear.

---

## 📏 5. The `width` and `height` Attributes

The `width` and `height` attributes specify the displayed width and height of an image. When written as numeric HTML attributes, their values represent CSS pixels.

### Example

```html
<img
    src="images/girl.jpg"
    alt="A girl wearing a jacket"
    width="300"
    height="200"
>
```

In this example:

- `width="300"` sets the image width to 300 CSS pixels.
- `height="200"` sets the image height to 200 CSS pixels.

These dimensions should generally match the image's intended aspect ratio to avoid stretching or distortion. CSS can also be used to control image dimensions.

---

## ♿ 6. The `alt` Attribute

The `alt` attribute provides **alternative text** for an image. It helps communicate the image's meaning when the image cannot be displayed and allows screen readers to describe meaningful images to users who cannot see them.

### Example

```html
<img src="img_typo.jpg" alt="Girl with a jacket">
```

If `img_typo.jpg` cannot be loaded, the browser may display the alternative text instead of the image.

### Why Is `alt` Important?

- **Accessibility:** Screen readers can announce the alternative text.
- **Fallback:** It provides useful information if the image fails to load.
- **Context:** It communicates the purpose or meaning of an image.

**Best practice:** Write descriptive alternative text for meaningful images. For decorative images that provide no useful information, use `alt=""`.

---

## 🎨 7. The `style` Attribute

The `style` attribute is used to apply **inline CSS** to an HTML element. It can control properties such as text color, font size, background color, alignment, and spacing.

### Example

```html
<p style="color: red;">This is a red paragraph.</p>
```

### More Examples

```html
<h1 style="color: blue;">Blue Heading</h1>

<p style="font-size: 20px;">Large paragraph text.</p>

<p style="background-color: yellow;">Yellow background.</p>
```

**Explanation:** CSS declarations are written inside the quotation marks. Each declaration consists of a property and a value separated by a colon, and multiple declarations are usually separated by semicolons.

For larger websites, external CSS stylesheets are generally easier to maintain than extensive inline styling.

---

## 🌍 8. The `lang` Attribute

The `lang` attribute specifies the primary language of an element's content. It is commonly included in the opening `<html>` tag to declare the language of the entire webpage.

This information helps browsers, search engines, translation tools, and assistive technologies interpret the page appropriately.

### Example: English

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>English Web Page</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
</body>
</html>
```

Here, `lang="en"` indicates that the page's primary language is English.

Other examples include:

- `lang="hi"` — Hindi
- `lang="or"` — Odia
- `lang="fr"` — French

**Best practice:** Specify the correct language using a valid language tag, preferably on the root `<html>` element.

---

## 💬 9. The `title` Attribute

The `title` attribute provides additional advisory information about an element. In many desktop browsers, this information appears as a tooltip when the user hovers over the element.

### Example

```html
<p title="I'm a tooltip">This is a paragraph.</p>
```

When a user hovers over the paragraph, the browser may display the text `I'm a tooltip`.

### Another Example

```html
<button title="Save your changes">Save</button>
```

The title provides extra information about the button's purpose.

**Important:** Do not rely on the `title` attribute as the only way to communicate essential information, because tooltips may not be accessible or available to every user.

---

## ⚠️ 10. Important Rules

1. Attributes are generally written inside the opening tag.
2. An attribute typically follows the format `attribute_name="attribute_value"`.
3. Use quotation marks around attribute values. Double quotes are the recommended convention.
4. Standard HTML attribute names are case-insensitive, but lowercase is recommended.
5. Attribute values are not always lowercase. For example, text in `title` and `alt` can use normal capitalization.
6. Some attributes are Boolean attributes, such as `required` and `disabled`, and do not need values like `"true"` or `"false"`.
7. An element can contain multiple attributes.
8. Attribute names and values must follow HTML syntax rules.
9. Use meaningful `alt` text for informative images.
10. The `href` attribute specifies a link destination, while `src` specifies the source of an embedded resource such as an image.

### Example: Multiple Attributes Together

```html
<a
    href="https://www.w3schools.com"
    title="Learn HTML"
    target="_blank"
    rel="noopener noreferrer"
>
    Learn HTML
</a>

<img
    src="images/girl.jpg"
    alt="A girl wearing a jacket"
    width="300"
    height="200"
>
```

---

## ⚡ 11. Quick Summary

| Attribute | Full Form / Meaning | Purpose |
|---|---|---|
| `href` | Hypertext Reference | Specifies a hyperlink destination. |
| `src` | Source | Specifies the location of a resource. |
| `width` | Width | Specifies an element's width, commonly an image's displayed width. |
| `height` | Height | Specifies an element's height, commonly an image's displayed height. |
| `alt` | Alternative Text | Provides a text alternative for an image. |
| `style` | Inline CSS styling | Applies CSS declarations to an element. |
| `lang` | Language | Identifies the language of the content. |
| `title` | Advisory title information | Provides additional information, often shown as a tooltip. |
| `target` | Browsing context | Specifies where a linked document should open. |

### 📝 One-Minute Revision

- **HTML attributes** add information or configure an element.
- **`href`** is used with links to specify their destination.
- **`src`** specifies an image or other resource's location.
- **Absolute URLs** provide complete addresses; **relative URLs** use a base URL.
- **`width` and `height`** specify image dimensions.
- **`alt`** improves image accessibility.
- **`style`** applies inline CSS.
- **`lang`** declares the content language.
- **`title`** supplies additional advisory information.

---

## 🧪 Practice Exercise

Create a webpage that includes:

- [x] An HTML document with `lang="en"`.
- [x] A link to an external website using `href`.
- [x] An image using `src`, `alt`, `width`, and `height`.
- [x] A paragraph with a red text color using `style`.
- [x] A paragraph with a `title` tooltip.
- [x] One relative link to another HTML file in your project.

<p align="center">
  <b>🚀 Understand attributes. Write meaningful HTML. Build better websites.</b>
  <br>
  <sub>Web Development Notes | HTML Fundamentals</sub>
</p>