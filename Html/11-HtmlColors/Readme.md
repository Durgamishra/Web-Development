# HTML Colors

HTML colors are used to change the appearance of web pages. Colors can be specified using predefined color names or different color value formats, such as RGB, HEX, HSL, RGBA, and HSLA.

## 1. Background Color

The `background-color` CSS property is used to set the background color of an HTML element.

**Example:**

```html
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color:DodgerBlue;">
  Hello World
</h1>

<p style="background-color:Tomato;">
  This is a paragraph.
</p>

</body>
</html>
```

**Explanation:**
- `background-color` sets the background color.
- `DodgerBlue` and `Tomato` are predefined CSS color names.
- The background color appears behind the content of the element.

## 2. Text Color

The `color` CSS property is used to change the color of text.

**Example:**

```html
<h1 style="color:Tomato;">Hello World</h1>

<p style="color:DodgerBlue;">Lorem ipsum dolor sit amet.</p>

<p style="color:MediumSeaGreen;">Welcome to HTML.</p>
```

**Explanation:**

The heading appears tomato-colored, the first paragraph appears blue, and the second paragraph appears green.

## 3. Border Color

The `border-color` CSS property is used to specify the color of an element's border. A border style must also be set for the border to be visible.

**Example:**

```html
<h1 style="border: 2px solid Tomato;">
  Tomato Border
</h1>

<p style="border: 3px solid DodgerBlue;">
  Blue Border
</p>

<p style="border: 2px solid MediumSeaGreen;">
  Green Border
</p>
```

**Explanation:**
- `border` specifies the border width, style, and color.
- `2px` or `3px` defines the border thickness.
- `solid` defines a continuous border line.
- The color name determines the border color.

## 4. HTML Color Values

Colors can be specified using five common formats.

### A. Color Names

CSS provides predefined color names, such as `Red`, `Blue`, `Green`, and `Tomato`.

```html
<h1 style="color:Red;">Red Heading</h1>
<p style="background-color:Yellow;">Yellow Background</p>
```

### B. RGB Values

RGB stands for **Red, Green, and Blue**. Each component generally ranges from 0 to 255.

**Syntax:** `rgb(red, green, blue)`

```html
<h1 style="color:rgb(255, 0, 0);">
  Red Text
</h1>

<p style="background-color:rgb(0, 0, 255);">
  Blue Background
</p>

<p style="border:2px solid rgb(0, 128, 0);">
  Green Border
</p>
```

Examples:
- `rgb(255, 0, 0)` — Red
- `rgb(0, 255, 0)` — Green
- `rgb(0, 0, 255)` — Blue
- `rgb(0, 0, 0)` — Black
- `rgb(255, 255, 255)` — White

### C. HEX Values

HEX stands for **Hexadecimal color notation**. It uses a `#` symbol followed by six hexadecimal digits representing red, green, and blue components.

**Syntax:** `#RRGGBB`

```html
<h1 style="color:#FF0000;">Red Text</h1>

<p style="background-color:#00FF00;">
  Green Background
</p>

<p style="border:2px solid #0000FF;">
  Blue Border
</p>
```

Examples:
- `#FF0000` — Red
- `#00FF00` — Green
- `#0000FF` — Blue
- `#000000` — Black
- `#FFFFFF` — White

### D. HSL Values

HSL stands for **Hue, Saturation, and Lightness**.

**Syntax:** `hsl(hue, saturation, lightness)`

- **Hue:** The color angle, usually from 0 to 360 degrees.
- **Saturation:** The intensity of the color, expressed as a percentage.
- **Lightness:** How light or dark the color is, expressed as a percentage.

```html
<h1 style="color:hsl(0, 100%, 50%);">
  Red Text
</h1>

<p style="background-color:hsl(120, 100%, 50%);">
  Green Background
</p>

<p style="border:2px solid hsl(240, 100%, 50%);">
  Blue Border
</p>
```

### E. RGBA Values

RGBA stands for **Red, Green, Blue, and Alpha**. The alpha component controls transparency, from `0` (fully transparent) to `1` (fully opaque).

**Syntax:** `rgba(red, green, blue, alpha)`

```html
<h1 style="color:rgba(255, 0, 0, 1);">
  Fully Opaque Red Text
</h1>

<p style="background-color:rgba(0, 0, 255, 0.5);">
  Semi-transparent Blue Background
</p>

<p style="border:3px solid rgba(0, 128, 0, 0.7);">
  Semi-transparent Green Border
</p>
```

### F. HSLA Values

HSLA stands for **Hue, Saturation, Lightness, and Alpha**. It adds transparency to the HSL color format.

**Syntax:** `hsla(hue, saturation, lightness, alpha)`

```html
<h1 style="color:hsla(0, 100%, 50%, 1);">
  Red Text
</h1>

<p style="background-color:hsla(240, 100%, 50%, 0.5);">
  Semi-transparent Blue Background
</p>

<p style="border:3px solid hsla(120, 100%, 25%, 0.8);">
  Green Border
</p>
```

## 5. Quick Revision Table

| Color Format | Meaning | Example |
|---|---|---|
| Color name | Predefined color name | `Tomato` |
| RGB | Red, Green, Blue | `rgb(255, 0, 0)` |
| HEX | Hexadecimal notation | `#FF0000` |
| HSL | Hue, Saturation, Lightness | `hsl(0, 100%, 50%)` |
| RGBA | RGB with alpha transparency | `rgba(255, 0, 0, 0.5)` |
| HSLA | HSL with alpha transparency | `hsla(0, 100%, 50%, 0.5)` |

## 6. Important Exam Questions

**Q1. What are HTML colors?**

HTML colors are colors applied to webpage elements using CSS. They can be specified using predefined color names, RGB, HEX, HSL, RGBA, and HSLA values.

**Q2. What is the difference between RGB and RGBA?**

RGB defines a color using red, green, and blue components, whereas RGBA adds an alpha component to control transparency.

**Q3. What is the difference between background color, text color, and border color?**

- `background-color` changes the background of an element.
- `color` changes the text color.
- `border-color` changes the color of an element's border.

**Q4. What does HSL stand for?**

HSL stands for Hue, Saturation, and Lightness.

**Q5. What is the purpose of alpha in RGBA and HSLA?**

Alpha controls the transparency of a color, ranging from `0` for fully transparent to `1` for fully opaque.

## 7. Important Note

Color properties are defined by CSS and applied to HTML elements through the `style` attribute or a CSS stylesheet. For example:

```html
<h1 style="color:Tomato;">Hello World</h1>
```

Here, `style` is the HTML attribute, while `color` is the CSS property and `Tomato` is its value.