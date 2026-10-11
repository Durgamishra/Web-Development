# 🎨 HTML Styles 
![HTML](https://img.shields.io/badge/HTML5-Styles-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-Styling-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Level](https://img.shields.io/badge/Level-Beginner-success?style=for-the-badge)

HTML styles are used to change the appearance and presentation of HTML elements on a webpage. They allow us to customize background colors, text colors, font styles, text sizes, alignment, and many other visual properties. HTML uses the `style` attribute to apply **inline CSS (Cascading Style Sheets)** directly to an element. CSS is the language responsible for controlling the design and layout of web pages, while HTML provides the structure and content. By combining HTML with CSS, developers can create webpages that are more attractive, readable, and user-friendly.

## 📑 Table of Contents

- [1. HTML Style Attribute](#1-html-style-attribute)
- [2. Background Color](#2-background-color)
- [3. Text Color](#3-text-color)
- [4. Font Family](#4-font-family)
- [5. Text Size](#5-text-size)
- [6. Text Alignment](#6-text-alignment)
- [7. Complete Example](#7-complete-example)
- [8. Important Points](#8-important-points)
- [9. Quick Summary](#9-quick-summary)
- [10. Practice Exercise](#10-practice-exercise)

---

## 1. HTML Style Attribute

The HTML `style` attribute is used to apply CSS properties directly to an HTML element. It allows developers to modify the visual appearance of individual elements without creating a separate CSS file. The attribute is written inside the opening tag, and its value contains a CSS property followed by a colon and its corresponding value. Each CSS declaration generally ends with a semicolon. For example, `style="color:blue;"` changes the text color of an element to blue.

### Syntax

```html
<tagname style="property: value;">
    Content goes here
</tagname>
```

### Example

```html
<h1 style="color: blue;">Welcome to HTML</h1>
<p style="font-size: 20px;">This is a styled paragraph.</p>
```

**Explanation:**
- `style` is the HTML attribute used to apply inline CSS.
- `color` and `font-size` are CSS properties.
- `blue` and `20px` are the corresponding property values.
- The `<h1>` and `<p>` elements display the content on the webpage.

**Note:** Inline CSS is useful for learning and small examples. For larger websites, internal or external CSS is usually better because it keeps the design organized and easier to maintain.

## 2. Background Color

The CSS `background-color` property defines the background color of an HTML element. It can be applied to the entire webpage by styling the `<body>` element or to individual elements such as headings, paragraphs, sections, and containers. Background colors can be specified using color names, hexadecimal values, RGB values, and other supported CSS color formats. Choosing appropriate background colors helps separate sections and improves the visual appearance of a webpage.

### Example

```html
<!DOCTYPE html>
<html>
<head>
    <title>Background Color</title>
</head>
<body style="background-color: powderblue;">

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

</body>
</html>
```

**Explanation:** The `background-color: powderblue;` declaration changes the background of the entire page's body to powder blue.

To apply a background color to just one element, use:

```html
<h1 style="background-color: yellow;">
    Welcome to My Website
</h1>

<p style="background-color: lightgray;">
    This paragraph has a gray background.
</p>
```

**Output:** The heading has a yellow background, while the paragraph has a light-gray background.

## 3. Text Color

The CSS `color` property defines the foreground color of text inside an HTML element. It can be used to change the color of headings, paragraphs, links, and other text content. Different colors can be used to highlight important information, establish visual hierarchy, and improve readability. However, text colors should always provide sufficient contrast against their backgrounds so that users can read the content comfortably.

### Example

```html
<h1 style="color: blue;">This is a heading</h1>

<p style="color: red;">
    This is a red paragraph.
</p>

<p style="color: green;">
    This is a green paragraph.
</p>
```

**Explanation:**
- `color: blue;` displays the heading text in blue.
- `color: red;` displays the paragraph text in red.
- `color: green;` displays the paragraph text in green.

You can also use hexadecimal color codes:

```html
<h1 style="color: #2563eb;">Blue Heading</h1>
<p style="color: #dc2626;">Red Paragraph</p>
```

Here, `#2563eb` and `#dc2626` are hexadecimal color values.

## 4. Font Family

The CSS `font-family` property specifies which font should be used to display text within an HTML element. Fonts influence the appearance, readability, and personality of a webpage. For example, Verdana is commonly associated with clear screen readability, while Courier is a monospaced font in which characters occupy equal horizontal space. Developers can specify multiple fonts as fallbacks so that the browser can use another available font if the preferred font is unavailable. Font names containing spaces should be placed inside quotation marks.

### Example

```html
<h1 style="font-family: Verdana, sans-serif;">
    This is a heading
</h1>

<p style="font-family: Courier, monospace;">
    This is a paragraph.
</p>
```

**Explanation:**
- `font-family: Verdana, sans-serif;` requests Verdana, with a generic sans-serif fallback.
- `font-family: Courier, monospace;` requests Courier, with a generic monospace fallback.

Another example:

```html
<p style="font-family: Arial, sans-serif;">
    This paragraph uses Arial.
</p>

<p style="font-family: Georgia, serif;">
    This paragraph uses Georgia.
</p>
```

**Important:** The browser may use a fallback font if the preferred font is not installed or otherwise available.

## 5. Text Size

The CSS `font-size` property controls the size of text displayed inside an HTML element. It can be specified using different units, including pixels (`px`), percentages (`%`), and relative units such as `em` and `rem`. A suitable font size improves readability and helps distinguish headings from paragraphs and other content. For example, `font-size: 30px;` specifies a font size of 30 pixels, while `font-size: 160%;` specifies a size relative to the applicable reference font size.

### Example using percentages

```html
<h1 style="font-size: 300%;">
    This is a heading
</h1>

<p style="font-size: 160%;">
    This is a paragraph.
</p>
```

### Example using pixels

```html
<h1 style="font-size: 36px;">
    Large Heading
</h1>

<p style="font-size: 18px;">
    Normal Paragraph
</p>

<p style="font-size: 14px;">
    Smaller Text
</p>
```

**Explanation:**
- `300%` requests a font size three times the applicable reference size.
- `160%` requests a font size 1.6 times the applicable reference size.
- `36px`, `18px`, and `14px` specify sizes in pixels.

**Note:** Percentage-based font sizes depend on the inherited or parent font size. For responsive websites, `rem` and other relative sizing techniques can also be useful.

## 6. Text Alignment

The CSS `text-align` property controls the horizontal alignment of inline content, such as text, within a block-level element. It supports values such as `left`, `right`, `center`, and `justify`. Left alignment is commonly used for paragraphs in English, center alignment is useful for titles, and right alignment may be used in particular layouts. Justified text adjusts spacing between words so that the text aligns with both edges of the available line width.

### Example

```html
<h1 style="text-align: center;">
    Centered Heading
</h1>

<p style="text-align: center;">
    This paragraph is centered.
</p>

<p style="text-align: left;">
    This paragraph is left-aligned.
</p>

<p style="text-align: right;">
    This paragraph is right-aligned.
</p>

<p style="text-align: justify;">
    This paragraph uses justified alignment. The browser adjusts
    the spacing between words so that the text aligns with both
    the left and right edges of the available space.
</p>
```

**Explanation:**
- `text-align: center;` centers the text.
- `text-align: left;` aligns the text to the left.
- `text-align: right;` aligns the text to the right.
- `text-align: justify;` adjusts line spacing between words to align the text with both edges.

## 7. Complete Example

The following program demonstrates background color, text color, font family, font size, and text alignment in a single HTML document.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Styles Example</title>
</head>

<body style="background-color: #f0f9ff;">

    <h1 style="color: #1d4ed8;
               font-family: Arial, sans-serif;
               font-size: 36px;
               text-align: center;">
        Welcome to HTML Styles
    </h1>

    <p style="color: #dc2626;
              font-family: Verdana, sans-serif;
              font-size: 20px;
              text-align: center;">
        This paragraph demonstrates text styling.
    </p>

    <p style="background-color: #dbeafe;
              color: #1e3a8a;
              font-size: 18px;
              text-align: left;">
        HTML provides structure, while CSS controls presentation.
    </p>

</body>
</html>
```

**Result:** The webpage has a light-blue background, a centered blue heading, a centered red paragraph, and a separate paragraph with a light-blue background.

## 8. Important Points

1. The `style` attribute is used to apply inline CSS to an HTML element.
2. CSS stands for **Cascading Style Sheets**.
3. `background-color` changes the background color of an element.
4. `color` changes the foreground or text color.
5. `font-family` specifies the font used to display text.
6. `font-size` controls the size of text.
7. `text-align` controls the horizontal alignment of text.
8. A CSS declaration follows the format `property: value;`.
9. Multiple CSS declarations can be written inside the same `style` attribute and separated by semicolons.
10. External CSS is generally recommended for styling larger websites because it improves reusability and maintainability.

## 9. Quick Summary

| CSS Property | Purpose | Example |
|---|---|---|
| `background-color` | Changes the element's background color | `background-color: yellow;` |
| `color` | Changes text color | `color: blue;` |
| `font-family` | Specifies the font | `font-family: Arial, sans-serif;` |
| `font-size` | Changes text size | `font-size: 20px;` |
| `text-align` | Aligns text horizontally | `text-align: center;` |

**Remember this syntax:**

```html
<tagname style="property: value;">
    Content
</tagname>
```

In short, HTML styles allow developers to improve the appearance of webpages using CSS properties. The `style` attribute provides a simple way to apply these properties directly to HTML elements. Background colors, text colors, font families, font sizes, and text alignment are some of the most fundamental styling techniques in web development.

## 10. Practice Exercise

Create a simple HTML webpage that satisfies all the following requirements:

- Set the webpage background color to light yellow.
- Create a heading with blue text, a font size of `36px`, and centered alignment.
- Create a paragraph with green text and a font size of `20px`.
- Set the paragraph's font family to Arial.
- Add another paragraph with a light-gray background.

**Learning objective:** After completing this exercise, you should be able to apply basic CSS properties to HTML elements using the inline `style` attribute.

---

**End of HTML Styles Notes**  
*Keep practicing — understanding these properties is the first step toward designing beautiful webpages with CSS.*