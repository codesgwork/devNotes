### CSS Specificity Explained

**Specificity** in CSS determines which rule is applied when multiple CSS rules target the same element. The browser calculates specificity as a weight based on the types of selectors used in a rule. The higher the specificity, the more priority that rule has over others.

### How Specificity Works

Each CSS selector can be broken down into four categories for calculating specificity:

1. **Inline styles** (e.g., styles defined within an element's `style` attribute)
2. **ID selectors** (e.g., `#example`)
3. **Class selectors**, attributes selectors, and pseudo-classes (e.g., `.class`, `[type="text"]`, `:hover`)
4. **Type selectors** and pseudo-elements (e.g., `div`, `h1`, `::before`)

### Specificity Calculation Formula

Specificity is often represented as a four-part value in the format `(a, b, c, d)`, where:

- **a**: Inline styles (if present, this is `1`, otherwise `0`)
- **b**: Number of ID selectors in the selector
- **c**: Number of class selectors, attribute selectors, and pseudo-classes
- **d**: Number of type selectors and pseudo-elements

The specificity values are compared from left to right. The higher number in any category will determine which rule takes precedence.

### Examples

1. **Element Selector** (`div`, `p`)

   - Specificity: `0, 0, 0, 1`
   - Explanation: One type selector (`div` or `p`).

2. **Class Selector** (`.example`)

   - Specificity: `0, 0, 1, 0`
   - Explanation: One class selector.

3. **ID Selector** (`#header`)

   - Specificity: `0, 1, 0, 0`
   - Explanation: One ID selector.

4. **Combination** (`#header .nav a`)

   - Specificity: `0, 1, 1, 1`
   - Explanation: One ID (`#header`), one class (`.nav`), and one type selector (`a`).

5. **Inline Styles** (`<div style="color: red;"></div>`)
   - Specificity: `1, 0, 0, 0`
   - Explanation: Inline styles always override other rules unless marked with `!important`.

### Comparing Specificity

If two or more rules apply to the same element, their specificity values are compared:

- Rule 1: `#header .nav` → Specificity: `0, 1, 1, 0`
- Rule 2: `.footer p` → Specificity: `0, 0, 1, 1`

Here, **Rule 1** has a higher specificity because it contains an ID selector, so it will take precedence.

### Specificity and `!important`

The `!important` declaration overrides specificity. However, if multiple rules use `!important`, the one with higher specificity will still win. Only inline styles with `!important` can override other rules marked with `!important`.

### Order of Precedence in Case of Ties

If two rules have the same specificity, the one that appears later in the stylesheet will be applied. This is called the **"cascade"** effect in CSS.

### Summary

1. **Inline styles** (`a`) > **ID selectors** (`b`) > **Class selectors, attributes, pseudo-classes** (`c`) > **Type selectors, pseudo-elements** (`d`)
2. Compare specificity values from left to right.
3. `!important` overrides specificity but can be overridden by inline styles marked as `!important`.

This helps you understand which styles get applied when multiple selectors target the same element.
