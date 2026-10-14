# HSL Color Values

HSL stands for **Hue, Saturation, and Lightness**. It is a color model used in CSS to specify colors based on their position on a color wheel, color intensity, and brightness.

The correct CSS syntax is:

```css
hsl(hue, saturation, lightness)
```

## 1. Hue

Hue represents the type of color and is measured in degrees on a color wheel, ranging from `0` to `360`.

Common hue values:

| Hue | Color |
|---:|---|
| `0°` | Red |
| `60°` | Yellow |
| `120°` | Green |
| `180°` | Cyan |
| `240°` | Blue |
| `300°` | Magenta |
| `360°` | Red |

**Example:**

```html
<h1 style="color:hsl(0, 100%, 50%);">Red</h1>

<h1 style="color:hsl(120, 100%, 50%);">Green</h1>

<h1 style="color:hsl(240, 100%, 50%);">Blue</h1>
```

**Explanation:** The hue determines which color is selected. For example, `120°` represents green.

## 2. Saturation

Saturation describes the intensity or purity of a color. It is expressed as a percentage from `0%` to `100%`.

- **100%:** Full, vivid color.
- **50%:** Less saturated color.
- **0%:** No saturation; the result is a shade of gray.

**Example:**

```html
<p style="color:hsl(0, 100%, 50%);">
    Red with 100% saturation
</p>

<p style="color:hsl(0, 50%, 50%);">
    Red with 50% saturation
</p>

<p style="color:hsl(0, 0%, 50%);">
    Gray with 0% saturation
</p>
```

**Explanation:** The hue and lightness remain the same, but changing saturation makes the color more vivid or more gray.

## 3. Lightness

Lightness describes how light or dark a color appears. It is expressed as a percentage from `0%` to `100%`.

- **0%:** Black.
- **50%:** The normal or pure hue at the selected saturation.
- **100%:** White.

**Example:**

```html
<p style="color:hsl(0, 100%, 0%);">
    Black
</p>

<p style="color:hsl(0, 100%, 50%);">
    Pure Red
</p>

<p style="color:hsl(0, 100%, 100%);">
    White
</p>
```

**Explanation:** With the hue and saturation fixed, changing lightness from `0%` to `100%` changes the color from black through red to white.

## 4. Complete HSL Example

```html
<!DOCTYPE html>
<html>
<head>
    <title>HSL Colors</title>
</head>
<body>

    <h1 style="color:hsl(0, 100%, 50%);">
        Red Heading
    </h1>

    <p style="background-color:hsl(120, 100%, 50%);">
        Green Background
    </p>

    <p style="background-color:hsl(240, 100%, 50%);">
        Blue Background
    </p>

    <p style="background-color:hsl(60, 100%, 50%);">
        Yellow Background
    </p>

</body>
</html>
```

## 5. HSLA Color Values

HSLA stands for **Hue, Saturation, Lightness, and Alpha**. It extends HSL by adding an alpha component to control transparency.

**Syntax:**

```css
hsla(hue, saturation, lightness, alpha)
```

The first three values define the color, while alpha determines its opacity.

### Alpha Range

- `0` — Fully transparent.
- `0.5` — 50% opacity.
- `1` — Fully opaque.

### Example

```html
<!DOCTYPE html>
<html>
<head>
    <title>HSLA Colors</title>
</head>
<body>

    <h1 style="color:hsla(0, 100%, 50%, 1);">
        Fully Opaque Red
    </h1>

    <p style="background-color:hsla(240, 100%, 50%, 0.5);">
        Semi-transparent Blue Background
    </p>

    <p style="background-color:hsla(120, 100%, 50%, 0);">
        Fully Transparent Green Background
    </p>

</body>
</html>
```

**Explanation:** In the second paragraph, the blue background has an alpha value of `0.5`, making it semi-transparent.

## 6. Difference Between HSL and HSLA

| HSL | HSLA |
|---|---|
| Stands for Hue, Saturation, Lightness. | Stands for Hue, Saturation, Lightness, Alpha. |
| Uses three components. | Uses four components. |
| Does not specify alpha transparency. | Specifies alpha transparency. |
| Example: `hsl(0, 100%, 50%)` | Example: `hsla(0, 100%, 50%, 0.5)` |

## 7. Important Exam Questions

**Q1. What is HSL in CSS?**

HSL stands for Hue, Saturation, and Lightness. It is a color model used to define colors in CSS using a hue angle and saturation and lightness percentages.

**Q2. What are the ranges of hue, saturation, and lightness?**

- Hue: `0°` to `360°`.
- Saturation: `0%` to `100%`.
- Lightness: `0%` to `100%`.

**Q3. What is the difference between saturation and lightness?**

Saturation determines the intensity or purity of a color, whereas lightness determines how light or dark the color appears.

**Q4. What is HSLA?**

HSLA stands for Hue, Saturation, Lightness, and Alpha. It is a CSS color format that adds transparency control to HSL.

**Q5. What happens when lightness is 0% or 100%?**

At `0%` lightness, the result is black. At `100%` lightness, the result is white, regardless of hue and saturation.

## 8. Quick Revision

Remember these three properties:

- **Hue = Which color?**
- **Saturation = How vivid is the color?**
- **Lightness = How light or dark is the color?**

Alpha controls transparency when using HSLA.