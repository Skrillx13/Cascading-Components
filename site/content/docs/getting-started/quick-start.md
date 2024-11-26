---
layout: docs
title: Quick Start
description: Quickly get started with CCA thanks to our production-ready JavaScript and CSS.
group: getting-started
toc: true
---

## 1. Create a new `.html` file

{{< callout info >}}
You can name this file anything, but if you wish for the file to be your landing page, name it `index.html`. This is also a recommended practice for project consistency.
{{< /callout >}}

Fill up the HTML file with the following structure. We include the `<meta name="viewport">` tag for our components to have proper responsive behavior in mobile devices.

``` html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My first CCA site</title>
</head>

<body>
  <p>Example paragraph</p>
</body>

</html>
```

## 2. Include CCA's JavaScript

Include our JavaScript to get started! You can also choose to include our CSS for pre-built components (something like Bootstrap, or Primer). We use jsDelivr as our primary CDN, but there are alternate CDN's incase jsDelivr fails.

Place the JavaScript link at the **end** of the closing `<body>` tag, and the CSS at the `<head>` like so:

``` html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Skrillx13/cascading-components/dist/1.3/cca.min.css"> <!-- Our compiled CSS -->
  <title>My first CCA site</title>
</head>

<body>
  <p>Example paragraph</p>
    <script src="https://cdn.jsdelivr.net/gh/Skrillx13/dist/1.3/cca.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script> <!-- Our bundled & compiled JavaScript -->
</body>

</html>
```

## 3. Make your first component

We have a prepared example you can use right here (This only works if you include our CSS) to test if CCA works.

{{< example >}}
<div class="dropdown">
  <button class="btn btn-primary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
    Click me!
  </button>
  <ul class="dropdown-menu">
    <li><a class="dropdown-item" href="#">Dropdown Item 1</a></li>
    <li><a class="dropdown-item" href="#">Dropdown Item 2</a></li>
    <li><a class="dropdown-item" href="#">Another dropdown item</a></li>
  </ul>
</div>
{{< /example >}}

## 4. Next Steps

Next, you can start [making your own CCA components](/docs/5.3/getting-started/your-first-component) by learning how to style, declare, and create advanced components.