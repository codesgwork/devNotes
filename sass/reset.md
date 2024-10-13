When it comes to **CSS Normalize** and **CSS Reset**, both aim to make web pages look consistent across different browsers, but they approach the problem differently:

### 1. **CSS Normalize:**

- **Purpose**: It preserves useful browser-specific styles and fixes inconsistencies in the default styling of HTML elements across browsers.
- **Use case**: Normalize is more refined because it doesn’t remove all styles; it keeps default styling when it’s useful.
- **Example**: It keeps the default margin for elements like `h1`, `p`, but fixes inconsistencies in font rendering, form elements, and more.

### 2. **CSS Reset:**

- **Purpose**: It removes all default styles applied by the browser, leaving you with a blank slate.
- **Use case**: CSS Reset is more aggressive, which is useful when you want complete control over the styling of your page from scratch.
- **Example**: It will remove all margins, paddings, and font sizes on elements like `body`, `h1`, `p`, etc.

  **Popular Reset CSS (Eric Meyer's Reset):**
  comment for header

  ```scss
  /* 
  RESET  STYLE CODE 
  NORMALIZE CSS
  */
  ```

```scss
*,
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  //Root font 1rem = 16px; default

  font-size: 62.5%; //new default // 1rem = 10px
  // Calculation => 10/16 = 62.5%
  //  1rem = 9px, 9/16 = 56.25%
  // 1rem = 8px, 8/16 = 50%
  // 1rem = 14px, 14/16 = 87.5%
  @include respond('ebook') {
    font-size: 56.25%;
  }
  @include respond('tablet') {
    font-size: 50%;
  }
}

body {
  font-family: $contentFont;
  box-sizing: border-box;
  background-color: $app-BG;
  color: $black;
  line-height: 1.6;
  font-size: 1.7rem;

  margin: 0 auto;
  max-width: 80%;

  @include respond('ebook') {
    background-color: $ebook-BG;
    // background-color: $appBG-50;

    margin: 0 auto;
    max-width: 85%;
  }
  @include respond('tablet') {
    background-color: $tablet-BG;
    // background-color: $appBG-50;
    margin: 0 auto;
    max-width: 85%;
  }
  @include respond('mobileL') {
    background-color: $mobileL-BG;
    // background-color: $appBG-50;
    margin: 0 auto;
    max-width: 90%;
  }
  @include respond('mobileP') {
    background-color: $mobileP-BG;
    // background-color: $appBG-50;
    margin: 0 auto;
    max-width: 90%;
  }
}

h1,
h2,
h3,
h4 {
  font-family: $titleFont;
  margin-bottom: 1.5rem;
  line-height: 1.5;
}
h1 {
  font-weight: 800;
  font-size: 3rem;
}

h2 {
  font-weight: 600;
  font-size: 2.5rem;
}

h3 {
  font-weight: 500;
  font-size: 2rem;
}

p {
  font-family: $titleFont;
  font-size: 1.7rem;
}

a {
  text-decoration: none;
  color: $grey-900;
}

li {
  list-style-type: none;
}

img {
  // width: 100%;
  object-fit: cover;
}

button {
  letter-spacing: 1px;
  padding: 1rem;
  border-style: none;
  font-family: $tagFont;
  font-size: 1.6rem;
  border-radius: 3px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;

  background-color: $grey-900;
  border: 1px solid $grey-300;
  color: $white;

  &:hover {
    background-color: $blue-500;
    color: $grey-100;
  }
  &:active {
    border: 1px solid $white;
    outline: none;
  }
}
```

### Key Differences:

- **Normalize.css** keeps some useful defaults (better for maintaining browser behavior with minor fixes).
- **Reset.css** wipes out all styles (better if you want full control over styling).

**Which to use?**

- If you want a minimal, controlled approach to fix cross-browser issues, go with **Normalize**.
- If you want a completely clean slate, choose **Reset**.

Do you want to apply one of these to your project?
