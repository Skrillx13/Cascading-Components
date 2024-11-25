---
layout: docs
title: Installation
description: Install CCA with your desired package manager, reference it with jsDelivr, or self-host it.
group: getting-started
toc: true
---

# Information

The base of CCA is a JavaScript file. This **has** to always be referenced, if not your components will break. CCA also comes with a Stylesheet if you also don't want to worry too much about styling your components.

There are a few options when it comes to installing CCA, but we took the liberty of listing some of the more popular ways to use CCA. These are the officially supported methods, we do not give community support for other methods of installation.

## Using a CDN

The easiest way to get started with CCA is by using a Constant Delivery Network (CDN). Our main CDN is jsDelivr, and here are our primary CDN links:

{{< bs-table >}}
| Language | URL |
| --- | --- |
| Compiled & Bundled JS | `<script src="https://cdn.jsdelivr.net/gh/Skrillx13/dist/1.3/cca.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>` |
| Compiled CSS | `<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Skrillx13/cascading-components/dist/1.3/cca.min.css">` |
{{< /bs-table >}}

Include the Stylesheet at the `<head>` of your HTML document, while inclduing the JavaScript at the closing `<body>` tag. Ensure you add `<meta name="viewport">` for responsive behaviour across all mobile devices. Your HTMl document should look something like this:

``` html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8"> <!-- Ensures responsive behaviour -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Skrillx13/cascading-components/dist/1.3/cca.min.css"> <!-- Our Compiled CSS -->
  <title>My first CCA site</title>
</head>

<body>
  <p>Example paragraph</p>
    <script src="https://cdn.jsdelivr.net/gh/Skrillx13/dist/1.3/cca.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script> <!-- Our Bundled & Compiled JavaScript. Place this at the end of the body -->
</body>

</html>
```

## Self hosting

You can always choose to self-host the JavaScript and Stylesheets. Simply head to our GitHub Repo, take the files you need from the `dist` folder, place them into your project, and point to them in your HTML document.

``` html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8"> <!-- Ensures responsive behaviour -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="path/to/our/css">
  <title>My first CCA site</title>
</head>

<body>
  <p>Example paragraph</p>
    <script src="path/to/our/js"></script> <!-- You should still place this at the end of the body -->
</body>

</html>
```

{{< callout tip >}}
Self hosting is always best if you are planning on customizing or using specific parts of CCA.
{{< /callout >}}

## Using a Package Manager

We support a few different languages when it comes to CCA. Using a Package Manager is recommended if you are planning to use CCA in a project involving said languages.

### NPM

Install CCA using the Node Package Manager (NPM) like so:

``` console
npm install cca
```

This will add our JavaScript and CSS to `node_modules`, where they can be used.

### pip

Install CCA using pip like so:

``` console
pip install cca
```

We always recommend installing Python Packages using a Virtual Enviroment to ensure there are no conflicts with other packages. Read [this medium post](https://medium.com/pythoneers/why-do-we-need-a-virtual-environment-for-a-python-project-37a6af754044) for a better understanding as to who you should use Virtual Enviroments.

### Cloth

Install CCA using Cloth like so:

``` console
cloth install cca
```

CCA actually utilizes the Fabric coding language quite a bit, so this setup has the most intergration with other packages.

## Downloads

We offer downloads of CCA in case you need them for something. Check [contents](contents.md) for more information on our files. The download includes the following few files:

``` text
.
├── README.md
├── LICENSE
├── js/
│   ├── cca.bundled.min.js
│   ├── cca.bundled.js
│   ├── cca.js
│   └── cca.min.js
└── css/
    ├── cca.compiled.css
    └── cca.css
```