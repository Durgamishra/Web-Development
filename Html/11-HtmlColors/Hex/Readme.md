# HTML Color Values (HEX)

HTML colors can be specified using hexadecimal (HEX) values. A HEX color value begins with a `#` symbol followed by six hexadecimal digits in the format `#RRGGBB`.

- **RR** represents the intensity of Red.
- **GG** represents the intensity of Green.
- **BB** represents the intensity of Blue.

Each pair of digits ranges from `00` to `FF` in hexadecimal, equivalent to `0` to `255` in decimal.

## 1. Syntax of HEX Colors

```css
#RRGGBB
```

Examples:

- Black: `#000000`
- White: `#FFFFFF`
- Red: `#FF0000`
- Green: `#00FF00`
- Blue: `#0000FF`
- Yellow: `#FFFF00`

## 2. Examples of HEX Colors in HTML

### A. Black Color

```html
<h1 style="color:#000000;">Black Text</h1>
```

**Explanation:** All three color components are `00`, so the resulting color is black.

### B. White Color

```html
<h1 style="background-color:#FFFFFF;">White Background</h1>
```

**Explanation:** All three color components are `FF`, giving maximum intensity to red, green, and blue and producing white.

### C. Blue Color

```html
<h1 style="color:#0000FF;">Blue Text</h1>
```

**Explanation:** Red and green have zero intensity (`00`), while blue has maximum intensity (`FF`).

### D. Red Color

```html
<p style="background-color:#FF0000;">Red Background</p>
```

### E. Green Color

```html
<p style="background-color:#00FF00;">Green Background</p>
```

## 3. HEX Color Reference Table

| Color | HEX Value |
|---|---|
| Black | `#000000` |
| White | `#FFFFFF` |
| Red | `#FF0000` |
| Green | `#00FF00` |
| Blue | `#0000FF` |
| Yellow | `#FFFF00` |
| Cyan | `#00FFFF` |
| Magenta | `#FF00FF` |

## 4. Eight-Digit HEX Values (Including Alpha)

HEX colors can also use eight digits in the format `#RRGGBBAA`, where the final two digits (`AA`) represent the alpha channel, which controls transparency.

**Syntax:**

```css
#RRGGBBAA
```

Examples:

- `#0000FF80` — Blue with approximately 50% opacity.
- `#FF0000FF` — Fully opaque red.
- `#00FF0000` — Fully transparent green.

**Explanation of `#0000FF80`:**

- `00` — Red component.
- `00` — Green component.
- `FF` — Blue component.
- `80` — Alpha component, approximately 50% opacity.

The alpha value `80` is hexadecimal for 128, which is approximately half of the maximum alpha value `255`.

**Example in HTML:**

```html
<div style="background-color:#0000FF80;">
    Semi-transparent blue background
</div>
```

## 5. Important Exam Questions

**Q1. What is a HEX color value in HTML?**

A HEX color value is a hexadecimal notation used in CSS to represent colors. It generally begins with `#` and contains six hexadecimal digits representing red, green, and blue components.

**Q2. What is the HEX value of black, white, and blue?**

- Black: `#000000`
- White: `#FFFFFF`
- Blue: `#0000FF`

**Q3. What is the format of an eight-digit HEX color?**

The format is `#RRGGBBAA`, where `RR`, `GG`, and `BB` represent red, green, and blue, while `AA` represents alpha transparency.

**Q4. What does `#0000FF80` represent?**

It represents blue with approximately 50% opacity.

**Remember:** Six-digit HEX (`#RRGGBB`) defines a color, while eight-digit HEX (`#RRGGBBAA`) also specifies its transparency.