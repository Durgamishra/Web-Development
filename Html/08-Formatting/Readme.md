# ✨ HTML Formatting Elements — Complete Guide

![HTML5](https://img.shields.io/badge/HTML5-Formatting-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Level](https://img.shields.io/badge/Level-Beginner-success?style=for-the-badge)

HTML formatting elements are used to change the appearance of text or indicate its meaning and importance on a webpage. They allow developers to display bold text, italic text, highlighted text, smaller text, deleted text, inserted text, and mathematical expressions. Some elements mainly change the visual appearance of text, while others provide semantic meaning that can help browsers and assistive technologies understand the content.

## 1. Bold Text — `<b>`

The `<b>` element displays text in **bold** without indicating that the text is more important than the surrounding content.

### Example

```html
<p>This is a <b>bold text</b> example.</p>
```

**Output:** This is a **bold text** example.

**Use:** To visually draw attention to keywords or terms without assigning special importance.

## 2. Important Text — `<strong>`

The `<strong>` element indicates that its content has strong importance, seriousness, or urgency. Browsers usually display this text in bold by default.

### Example

```html
<p><strong>Warning:</strong> Do not switch off the computer.</p>
```

**Output:** **Warning:** Do not switch off the computer.

**Use:** Warnings, critical instructions, and important information.

**Difference:** `<b>` draws attention visually, whereas `<strong>` gives the text semantic importance.

## 3. Italic Text — `<i>`

The `<i>` element represents text set apart from normal prose, such as a technical term, a foreign-language phrase, or a thought. Browsers typically display it in italic style.

### Example

```html
<p>The scientific name is <i>Homo sapiens</i>.</p>
```

**Output:** The scientific name is *Homo sapiens*.

**Use:** Scientific names, foreign phrases, and terms that are stylistically distinct from the surrounding text.

## 4. Emphasized Text — `<em>`

The `<em>` element indicates stress emphasis. Browsers generally display emphasized text in italics, and assistive technologies may convey the emphasis.

### Example

```html
<p>You <em>must</em> complete your assignment today.</p>
```

**Output:** You *must* complete your assignment today.

**Use:** To emphasize a word or phrase that changes the intended meaning or stress of a sentence.

**Difference:** `<i>` marks text set apart from the surrounding prose, while `<em>` indicates emphasis.

## 5. Marked Text — `<mark>`

The `<mark>` element highlights text that is relevant to the current context. Browsers typically display it with a yellow background.

### Example

```html
<p>Remember to study <mark>HTML formatting elements</mark>.</p>
```

**Output:** Remember to study ==HTML formatting elements==.

**Use:** Highlighting search results, important terms in study notes, or relevant portions of a document.

## 6. Smaller Text — `<small>`

The `<small>` element represents side comments, fine print, or other content that is less prominent than the surrounding text. Browsers typically display it in a smaller font size.

### Example

```html
<p>Price: ₹500</p>
<p><small>Terms and conditions apply.</small></p>
```

**Output:** Price: ₹500

*Terms and conditions apply.* (displayed in smaller text)

**Use:** Copyright notices, disclaimers, and fine print.

## 7. Deleted Text — `<del>`

The `<del>` element represents text that has been deleted from a document. Browsers typically display it with a line through the text.

### Example

```html
<p>Original price: <del>₹1000</del></p>
<p>Discounted price: ₹700</p>
```

**Output:** Original price: ~~₹1000~~

Discounted price: ₹700

**Use:** Showing removed content, previous prices, or revisions in a document.

## 8. Inserted Text — `<ins>`

The `<ins>` element represents text that has been inserted into a document. Browsers typically display it with an underline.

### Example

```html
<p>My favorite color is <del>red</del> <ins>blue</ins>.</p>
```

**Output:** My favorite color is ~~red~~ <ins>blue</ins>.

**Use:** Showing additions or changes made to a document.

**Note:** `<del>` and `<ins>` are especially useful together when showing edits or revisions.

## 9. Subscript Text — `<sub>`

The `<sub>` element displays text below the normal text baseline. It is commonly used in chemical formulas and mathematical notation.

### Example

```html
<p>Water formula: H<sub>2</sub>O</p>
<p>Carbon dioxide: CO<sub>2</sub></p>
```

**Output:**
- Water formula: H₂O
- Carbon dioxide: CO₂

**Use:** Chemical formulas and other notation requiring subscripts.

## 10. Superscript Text — `<sup>`

The `<sup>` element displays text above the normal text baseline. It is commonly used for powers, exponents, and footnote markers.

### Example

```html
<p>Square of 5: 5<sup>2</sup> = 25</p>
<p>Cube of 3: 3<sup>3</sup> = 27</p>
```

**Output:**
- Square of 5: 5² = 25
- Cube of 3: 3³ = 27

**Use:** Mathematical powers, exponents, and certain footnote markers.

## 11. Complete HTML Program

The following program demonstrates all ten formatting elements in a single webpage.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Formatting Elements</title>
</head>
<body>

    <h1>HTML Formatting Elements</h1>

    <p>This is <b>bold text</b>.</p>

    <p>This is <strong>important text</strong>.</p>

    <p>This is <i>italic text</i>.</p>

    <p>This is <em>emphasized text</em>.</p>

    <p>This is <mark>marked text</mark>.</p>

    <p>This is <small>smaller text</small>.</p>

    <p>This is <del>deleted text</del>.</p>

    <p>This is <ins>inserted text</ins>.</p>

    <p>Water formula: H<sub>2</sub>O</p>

    <p>Mathematical expression: x<sup>2</sup></p>

</body>
</html>
```

## 12. Quick Summary

| HTML Element | Purpose | Default Appearance |
|---|---|---|
| `<b>` | Draws visual attention | Bold |
| `<strong>` | Indicates strong importance | Bold |
| `<i>` | Marks text set apart from normal prose | Italic |
| `<em>` | Indicates stress emphasis | Italic |
| `<mark>` | Highlights relevant text | Usually yellow background |
| `<small>` | Represents fine print or side comments | Smaller text |
| `<del>` | Represents deleted content | Strikethrough |
| `<ins>` | Represents inserted content | Underlined |
| `<sub>` | Displays subscript text | Below baseline |
| `<sup>` | Displays superscript text | Above baseline |

### Important Points for Exams

1. HTML formatting elements modify the appearance or meaning of text.
2. `<b>` and `<strong>` usually look similar, but `<strong>` conveys importance.
3. `<i>` and `<em>` usually look similar, but `<em>` conveys stress emphasis.
4. `<mark>` highlights relevant text.
5. `<small>` displays fine print or side comments.
6. `<del>` represents deleted content, while `<ins>` represents inserted content.
7. `<sub>` is used for expressions such as H₂O.
8. `<sup>` is used for expressions such as x².
9. The default appearance can be changed using CSS.
10. Semantic meaning should guide the choice between visually similar formatting elements.

**Conclusion:** HTML formatting elements help developers present information clearly and meaningfully. Understanding these ten elements is an important foundation for creating readable webpages, study notes, and well-structured HTML documents.