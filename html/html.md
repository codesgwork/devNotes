To include a favicon in an HTML file, you need to add a `<link>` element inside the `<head>` section of your HTML document. The favicon is usually a small icon that appears in the browser tab next to the page title.

Here’s how to include a favicon:

```html
<head>
    <link rel="icon" type="image/png" href="path/to/favicon.png">
</head>
```

### Explanation:
- `rel="icon"`: Specifies that this link is for the favicon.
- `type="image/png"`: Defines the image type. Common types include `image/png`, `image/x-icon`, and `image/svg+xml` based on your favicon format.
- `href="path/to/favicon.png"`: The path to your favicon image file. Replace this with the actual file path or URL of the favicon.

You can also use an `.ico` file or other formats as needed. Here’s an example with an `.ico` file:

```html
<head>
    <link rel="icon" type="image/x-icon" href="path/to/favicon.ico">
</head>
```

Make sure that the favicon file is available at the specified path, and your browser will display it accordingly.