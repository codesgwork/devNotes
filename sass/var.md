## variables

In SCSS, you can set variables using the `$` symbol followed by the variable name.

Variables can store values like colors, font sizes, spacing, etc., which can be reused throughout the stylesheet.

Here's the basic syntax:

```scss
// Defining variables
$primary-color: #3498db;
$font-size: 16px;
$padding: 20px;

// Using variables
body {
  font-size: $font-size;
  background-color: $primary-color;
  padding: $padding;
}
```

Once a variable is defined, you can use it anywhere in your SCSS file, making it easier to maintain and update styles. When you want to change a value, you only need to update the variable, and all occurrences will automatically reflect the change.

Would you like to try setting some SCSS variables for your project?

```scss
// font-family: "Montserrat", sans-serif;
// font-family: "Lato", sans-serif;
// font-family: "Poppins", sans-serif;

$logoFont: 'Dancing Script', cursive, 'Montserrat', sans-serif;
$titleFont: 'Montserrat', sans-serif;
$tagFont: 'Lato', sans-serif;
$contentFont: 'Poppins', sans-serif;

$app-BG: #fafafa;
$grey-100: #f1f5f9;
$grey-200: #e2e8f0;
$grey-300: #cbd5e1;
$grey-400: #94a3b8;
$grey-500: #64748b;
$grey-600: #475569;
$grey-700: #334155;
$grey-800: #1e293b;
$grey-900: #0f172a;
$blue-500: #2196f3;
$blue-700: #1976d2;
$blue-900: #0d47a1;
$red: #f45d5d;
$white: #fff;
$black: #222;

$radius: 0.4rem;
$spacing: 1px;
$transition: 0.3s ease-in-out all;

$max-width: 80%;
$fixed-width: 60rem;
$small: 1.3rem;

$shadow-1: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(208, 201, 201, 0.06);

$shadow-2: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);

$shadow-3: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);

$shadow-4: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);

// Variables for Breakpoints
// 1 em = 16px

//80em = Max width for small desktop screens
$ebook: 80em; // 1280px;

//64em = Max width for tablets
$tablet: 60em; // 960px;

// 48em = Max width for mobileL devices
$mobileL: 45em; // 720px

// 26em = Max width for mobileP devices
$mobileP: 28em; // 448px

//  BG color for test
$ebook-BG: #cfd8dc;
$tablet-BG: #c8e6c9;
$mobileL-BG: #b3e5fc;
$mobileP-BG: #ffebee;
```
