# 🏷️ HTML Headings

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Headings-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Topic-HTML%20Fundamentals-0EA5E9?style=for-the-badge" alt="HTML Fundamentals">
  <img src="https://img.shields.io/badge/Level-Beginner-22C55E?style=for-the-badge" alt="Beginner">
</p>

**HTML headings** are used to define titles and subtitles on a webpage. HTML provides six heading elements, ranging from `<h1>` to `<h6>`. The `<h1>` element represents the highest-level heading, while `<h6>` represents the lowest-level heading. Headings organize information into a meaningful hierarchy, making webpages easier to read, understand, navigate, and maintain.

## 📑 Table of Contents

- [1. HTML Heading Tags](#-1-html-heading-tags)
- [2. Example of All Six Headings](#-2-example-of-all-six-headings)
- [3. Why Are Headings Important?](#-3-why-are-headings-important)
- [4. Proper Heading Hierarchy](#-4-proper-heading-hierarchy)
- [5. Headings and SEO](#-5-headings-and-seo)
- [6. Changing Heading Sizes](#-6-changing-heading-sizes)
- [7. Common Mistakes](#-7-common-mistakes)
- [8. Quick Summary](#-8-quick-summary)

---

## 🧩 1. HTML Heading Tags

HTML contains six heading tags: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, and `<h6>`. Each tag represents a different level in the document's heading hierarchy.

| Tag | Description | Common Use |
|---|---|---|
| `<h1>` | Highest-level heading | Main page title |
| `<h2>` | Second-level heading | Major sections |
| `<h3>` | Third-level heading | Subsections |
| `<h4>` | Fourth-level heading | Sections within subsections |
| `<h5>` | Fifth-level heading | Lower-level sections |
| `<h6>` | Sixth-level heading | Lowest-level sections |

By default, browsers usually display headings in bold text, with `<h1>` larger than `<h2>`, and so on. Their appearance can be customized using CSS.

---

## 💻 2. Example of All Six Headings

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Headings Example</title>
</head>
<body>

    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>

</body>
</html>
```

### 🔍 Explanation

- `<h1>` defines the main heading of the page or a prominent top-level title.
- `<h2>` defines a major section under the main heading.
- `<h3>` defines a subsection within an `<h2>` section.
- `<h4>` defines a subsection within an `<h3>` section.
- `<h5>` defines a lower-level subsection within an `<h4>` section.
- `<h6>` defines the lowest heading level in HTML.

---

## 🎯 3. Why Are Headings Important?

Headings are important because they organize content into logical sections and help users understand the purpose of each part of a webpage. Many users scan a page rather than reading every word, so descriptive headings help them find relevant information quickly. Headings also provide a meaningful document structure that can help assistive technologies communicate how the content is organized.

### Main Benefits

- **Readability:** Makes long content easier to scan and understand.
- **Organization:** Separates a webpage into meaningful sections.
- **Accessibility:** Helps screen-reader users navigate between headings.
- **SEO:** Helps search engines interpret the page's content and structure.
- **Maintainability:** Makes documents easier for developers to update.

---

## 🌳 4. Proper Heading Hierarchy

Headings should follow a logical hierarchy. Usually, use `<h1>` for the page title, `<h2>` for main sections, and `<h3>` for subsections within those sections.

### Example

```html
<h1>Web Development</h1>

<h2>HTML</h2>
<p>HTML defines the structure of webpages.</p>

<h3>HTML Headings</h3>
<p>Headings organize webpage content.</p>

<h3>HTML Paragraphs</h3>
<p>Paragraphs represent blocks of text.</p>

<h2>CSS</h2>
<p>CSS controls the presentation of webpages.</p>

<h3>CSS Colors</h3>
<p>CSS colors customize the appearance of elements.</p>
```

### Visual Structure

```text
Web Development (h1)
├── HTML (h2)
│   ├── HTML Headings (h3)
│   └── HTML Paragraphs (h3)
└── CSS (h2)
    └── CSS Colors (h3)
```

**Important:** Choose heading levels based on their structural meaning, not simply their default font size. Avoid skipping levels unnecessarily, such as jumping from `<h2>` directly to `<h5>`.

---

## 🔍 5. Headings and SEO

SEO stands for **Search Engine Optimization**. It refers to practices that help search engines discover, understand, and present webpages in relevant search results.

HTML headings contribute to SEO by describing the topics and organization of a webpage. Clear, relevant headings help both readers and search engines understand what each section covers.

### SEO Best Practices

1. Use a clear and descriptive main heading.
2. Organize major topics with `<h2>` elements.
3. Use `<h3>` elements for related subsections.
4. Write headings that accurately describe the following content.
5. Avoid repeating keywords unnaturally just to influence rankings.
6. Do not use heading tags only to make text larger or bolder.

**Note:** Correct heading structure is useful for accessibility and content organization, but it does not guarantee higher search rankings.

---

## 🎨 6. Changing Heading Sizes

HTML defines the meaning and structure of headings, while CSS controls their visual appearance. You can change a heading's size, color, font, and spacing without changing its semantic level.

### Example

```html
<h1 style="font-size: 40px; color: darkblue;">
    Welcome to HTML
</h1>

<h2 style="font-size: 28px; color: green;">
    HTML Fundamentals
</h2>
```

Even if an `<h2>` is styled to appear larger than an `<h1>`, it remains a second-level heading in the document structure.

---

## ⚠️ 7. Common Mistakes

| Mistake | Better Practice |
|---|---|
| Using headings only to make text bold | Use CSS for visual styling. |
| Skipping heading levels without a reason | Maintain a logical hierarchy. |
| Using vague headings such as "Section 1" everywhere | Use descriptive headings. |
| Placing unrelated content under a heading | Keep each section focused on its topic. |
| Assuming headings automatically improve rankings | Focus on clear structure and useful content. |

---

## ⚡ 8. Quick Summary

- HTML provides six heading elements, from `<h1>` to `<h6>`.
- `<h1>` is the highest-level heading, and `<h6>` is the lowest-level heading.
- Headings define the structure and hierarchy of webpage content.
- Use `<h1>` for the main page title and `<h2>` for major sections.
- Use `<h3>` and lower-level headings for nested subsections.
- Headings improve readability, navigation, accessibility, and content organization.
- Search engines can use heading structure to better understand webpage content.
- Use CSS to customize heading appearance instead of choosing a heading level based on size alone.

### 🧪 Practice Exercise

Create a webpage about **Computer Science** that includes:

- [ ] One `<h1>` for the page title.
- [ ] Three `<h2>` elements for major subjects.
- [ ] At least two `<h3>` elements under one major subject.
- [ ] A paragraph under each heading.
- [ ] CSS to change the color and size of the main heading.

<p align="center">
  <b>🚀 Structure your content. Improve readability. Build accessible websites.</b>
  <br>
  <sub>Web Development Notes | HTML Fundamentals</sub>
</p>