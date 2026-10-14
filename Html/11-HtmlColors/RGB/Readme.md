# RGB Colors

RGB stands for **Red, Green, and Blue**. In HTML, colors can be specified using the CSS `rgb()` function, which combines different intensities of red, green, and blue to produce a particular color.

## 1. Syntax of RGB Colors

```css
rgb(red, green, blue)
```

**Range:** Each component can have an integer value from `0` to `255`.

- `0` means no intensity of that color component.
- `255` means maximum intensity of that color component.

## 2. Examples of RGB Colors

### A. Red Color

```html
<h1 style="color:rgb(255, 0, 0);">Red Color</h1>
```

**Explanation:** Red is at maximum intensity (`255`), while green and blue are both `0`. Therefore, the resulting color is red.

### B. Black Color

```html
<h1 style="color:rgb(0, 0, 0);">Black Color</h1>
```

**Explanation:** All three color components are `0`, so the resulting color is black.

### C. White Color

```html
<h1 style="color:rgb(255, 255, 255);">White Color</h1>
```

**Explanation:** All three color components are at maximum intensity (`255`), producing white.

### D. Green Color

```html
<h1 style="color:rgb(0, 255, 0);">Green Color</h1>
```

### E. Blue Color

```html
<h1 style="color:rgb(0, 0, 255);">Blue Color</h1>
```

## 3. RGB Color Reference Table

| RGB Value | Resulting Color |
|---|---|
| `rgb(255, 0, 0)` | Red |
| `rgb(0, 255, 0)` | Green |
| `rgb(0, 0, 255)` | Blue |
| `rgb(0, 0, 0)` | Black |
| `rgb(255, 255, 255)` | White |
| `rgb(255, 255, 0)` | Yellow |
| `rgb(255, 165, 0)` | Orange |

# Usage of Alpha

Alpha is used to control the **transparency of a color**, not its intensity. It is commonly used with the `rgba()` and `hsla()` CSS functions.

## 4. RGBA Syntax

```css
rgba(red, green, blue, alpha)
```

The first three values specify the color, while the fourth value specifies its transparency.

**Alpha range:** `0` to `1`.

- `0` — fully transparent.
- `0.5` — 50% opacity (semi-transparent).
- `1` — fully opaque.

## 5. Examples of Alpha

### A. Fully Opaque Color

```html
<p style="background-color:rgba(255, 99, 71, 1);">
  Fully opaque tomato color
</p>
```

### B. Semi-transparent Color

```html
<p style="background-color:rgba(255, 99, 71, 0.5);">
  Semi-transparent tomato color
</p>
```

**Explanation:** `rgb(255, 99, 71)` specifies a tomato-like color, and the alpha value `0.5` makes it semi-transparent.

### C. Fully Transparent Color

```html
<p style="background-color:rgba(255, 99, 71, 0);">
  Transparent background
</p>
```

**Explanation:** The background color becomes fully transparent, allowing the background behind it to show through.

## 6. Complete HTML Example

```html
<!DOCTYPE html>
<html>
<head>
    <title>RGB and Alpha Colors</title>
</head>
<body>

    <h1 style="color:rgb(255, 0, 0);">
        Red Text
    </h1>

    <p style="background-color:rgb(0, 255, 0);">
        Green Background
    </p>

    <p style="background-color:rgba(255, 99, 71, 0.5);">
        Semi-transparent Tomato Background
    </p>

</body>
</html>
```

## 7. Important Exam Questions

**Q1. What is RGB?**

RGB stands for Red, Green, and Blue. It is a color model used in CSS to specify colors by combining the intensities of these three components, each ranging from 0 to 255 when using integer values.

**Q2. What is the RGB value of black and white?**

- Black: `rgb(0, 0, 0)`
- White: `rgb(255, 255, 255)`

**Q3. What is alpha in RGBA?**

Alpha is the fourth component in RGBA. It controls color transparency and ranges from 0 (fully transparent) to 1 (fully opaque).

**Q4. What is the difference between RGB and RGBA?**

RGB uses three components—red, green, and blue—whereas RGBA adds a fourth component, alpha, to control transparency.

**Remember:** RGB controls the color components; alpha controls transparency.