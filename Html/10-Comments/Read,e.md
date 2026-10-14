# HTML Comments

## 1. HTML Comments

HTML comments are used to add notes or explanations inside HTML code. They help developers understand the purpose of the code and remember important information.

Comments are not displayed on the webpage in the browser.

**Syntax:**
```html
<!-- This is a comment -->
```

**Example:**
```html
<!-- This is a comment -->

<p>This is a paragraph.</p>

<!-- Remember to add more information here -->
```

**Explanation:**
- `<!--` marks the beginning of a comment.
- `-->` marks the end of a comment.
- Anything written between these symbols is treated as a comment.
- Comments help make code easier to read and maintain.

## 2. Hiding Content Using HTML Comments

HTML comments can temporarily hide HTML code from being rendered in the browser. This can be useful when testing code or debugging a webpage.

**Example:**
```html
<p>This is a paragraph.</p>

<!-- <p>This is another paragraph.</p> -->

<p>This is a paragraph too.</p>
```

**Output:**
```text
This is a paragraph.

This is a paragraph too.
```

**Explanation:**

The second paragraph is inside an HTML comment, so the browser does not display it as webpage content. The code remains in the HTML source and can be restored by removing the comment markers.

**Note:** Comments do not provide security. Hidden code can still be viewed by anyone who inspects the page source.

## 3. Hiding Inline Content

HTML comments can also be used to temporarily hide content in the middle of HTML code.

**Example:**
```html
<p>
  HTML is easy to learn.
  <!-- This content is temporarily hidden. -->
  HTML is used to create webpages.
</p>
```

**Explanation:**

The browser displays the text outside the comment but does not display the text inside it. This allows developers to temporarily exclude specific content without removing it from the source code.

## 4. Advantages of HTML Comments

1. **Code documentation:** Explain the purpose of different sections of code.
2. **Readability:** Make HTML code easier to understand.
3. **Debugging:** Temporarily disable sections of HTML while testing.
4. **Maintenance:** Help developers remember important details when updating code.

## 5. Important Points for Exams

- HTML comments begin with `<!--` and end with `-->`.
- Comments are not displayed as webpage content.
- Comments can contain notes, explanations, or temporarily disabled HTML code.
- HTML comments can be written on a single line or across multiple lines.
- Comments are visible in the page source and must not contain passwords or other secrets.

## 6. Short Exam Answer

**Q. What are HTML comments?**

HTML comments are statements written inside `<!--` and `-->` that are ignored by the browser when rendering webpage content. They are used to document code, improve readability, and temporarily hide HTML elements during testing or debugging.

**Q. What is the syntax of an HTML comment?**

```html
<!-- Write your comment here -->
```