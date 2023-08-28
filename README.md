# 🔥 Head

Welcome to the Head project, a comprehensive guide to HTML `<head>` tags.

## Table of Contents

- [Introduction](#introduction)
- [Recommended Minimum](#recommended-minimum)
- [Meta tags](#meta-tags)
- [Link tags](#link-tags)
- [Social Media](#social-media)
- [Extra](#extra)
- [License](#📝-license)

# Introduction

## Recommended Minimum

```html
<!DOCTYPE html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Page's Title</title>
</head>
<body>
  <!-- Content -->
</body>
```

### Charset Attribute

Specifies the character encoding for the HTML document. **`"utf-8"`** is the standard encoding that supports a wide range of characters.

```html
<meta charset="utf-8">
```

[MDN Charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset)

### Viewport Meta Tag

Configures the viewport properties to control how a webpage is displayed on different devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

[MDN Viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag)

### Title Tag

Defines the document's title that is shown in a browser's title bar or a page's tab.

```html
<title>Page's Title</title>
```

[MDN Viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title)


## Meta Tags

### Name Attributes

#### Application Name

The `application-name` meta tag specifies the name of the web application.

```html
<meta name="application-name" content="Your App Name">
```

Learn more: [MDN application-name](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name)

#### Author

The `author` meta tag specifies the author of the web page.

```html
<meta name="author" content="Author's Name">
```

Learn more: [MDN author](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name)

#### Description

The `description` meta tag provides a brief summary of the page's content, often used by search engines and social media platforms.

```html
<meta name="description" content="A concise description of the page">
```

Learn more: [MDN description](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name)

#### Referrer

The `referrer` meta tag specifies the referrer policy for the page.

```html
<meta name="referrer" content="no-referrer">
```

Learn more: [MDN referrer](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referer)

#### Color Scheme

The `color-scheme` meta tag sets the preferred color scheme for the page.

```html
<meta name="color-scheme" content="light dark">
```

Learn more: [MDN color-scheme](https://developer.mozilla.org/en-US/docs/Web/CSS/color-scheme)

#### Theme Color

The `theme-color` meta tag defines the color of the browser's UI elements when the page is active.

```html
<meta name="theme-color" content="#RRGGBB">
```

Learn more: [MDN theme-color](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name/theme-color)

### HTTP-Equiv Attributes

#### Content Security Policy

The `content-security-policy` meta tag specifies the content security policy for the page.

```html
<meta http-equiv="Content-Security-Policy" content="default-src 'self'">
```

Learn more: [MDN Content Security Policy](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP)

#### Refresh

The `refresh` meta tag automatically refreshes the page after a specified time interval.

```html
<meta http-equiv="refresh" content="5">
```

Learn more: [MDN Refresh](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#http-equiv)

## Link

### Stylesheet

The `rel="stylesheet"` link tag links an external stylesheet to the document for styling purposes.

```html
<link rel="stylesheet" href="styles.css">
```

Learn more: [MDN rel="stylesheet"](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel#stylesheet)

### Canonical URL

The `rel="canonical"` link tag specifies the canonical URL for the document to avoid duplicate content issues.

```html
<link rel="canonical" href="canonical-url.html">
```

Learn more: [MDN rel="canonical"](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel#canonical)

### Manifest for Web Application

The `rel="manifest"` link tag specifies the location of the web app's manifest file.

```html
<link rel="manifest" href="manifest.json">
```

Learn more: [MDN rel="manifest"](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel#manifest)

### Alternate to Another Language

The `rel="alternate"` link tag provides alternate versions of the current document in different languages.

```html
<link rel="alternate" hreflang="es" href="alternate-language.html">
```

Learn more: [MDN rel="alternate"](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link#alternate)

### RSS Feed

The `rel="alternate"` link tag can also be used to specify an RSS feed for the document.

```html
<link rel="alternate" type="application/rss+xml" title="RSS Feed" href="rss-feed.xml">
```

Learn more: [MDN rel="alternate"](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link#alternate)

### Icons

Icon-related link tags can be used to specify various icons for the document.

- Favicon:
  ```html
  <link rel="icon" href="favicon.ico">
  ```
- Apple Touch Icon:
  ```html
  <link rel="apple-touch-icon" href="apple-touch-icon.png">
  ```
- Mask Icon:
  ```html
  <link rel="mask-icon" href="mask-icon.svg" color="#000000">
  ```

Learn more: [MDN rel="icon"](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel#icon), [Apple Developer rel="apple-touch-icon"](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html#//apple_ref/doc/uid/TP40002051-CH3-SW4), [MDN rel="mask-icon"](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link#attr-rel)

### Conditional Loading with Media Queries

Load stylesheets conditionally based on media queries.

```html
<link rel="stylesheet" media="(max-width: 600px)" href="mobile.css">
<link rel="stylesheet" media="(min-width: 601px)" href="desktop.css">
```

Learn more: [MDN Media Queries](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link#media)

### Preloading Resources

Preload resources for improved performance.

```html
<link rel="preload" href="font.woff2" as="font" type="font/woff2" crossorigin>
<link rel="preload" href="image.jpg" as="image">
```

Learn more: [MDN rel="preload"](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel/preload)

### Prefetching Resources

Prefetch resources for upcoming navigations.

```html
<link rel="prefetch" href="next-page.html">
```

Learn more: [MDN rel="prefetch"](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel/prefetch)

## Social Media

### Open Graph and Twitter Card Tags

Facebook Open Graph tags customize content appearance when shared on social media platforms like Facebook, while Twitter Card tags enhance previews on Twitter.

#### `prefix` Attribute for Open Graph Tags

The `prefix` attribute defines a special marker for Open Graph (OG) meta tags in an HTML document. It's like a label that tells browsers and social media sites to treat `property` attributes beginning with `og:` as Open Graph details.

By adding `prefix="og:"` to your HTML, you ensure that anything with `og:` is recognized as Open Graph information. This helps browsers and platforms understand your content better.

```html
<head prefix="og: http://ogp.me/ns#">
  <!-- ... -->
</head>
```

#### og:url

The URL of the shared content.

```html
<meta property="og:url" content="https://example.com/page">
```

#### og:type

The type of the content, e.g., "website" or "article".

```html
<meta property="og:type" content="article">
```

#### og:title

The title of the shared content.

```html
<meta property="og:title" content="Page Title">
```

#### og:description

The description of the shared content.

```html
<meta property="og:description" content="Description of the content">
```

#### og:image

An image to display when the content is shared.

```html
<meta property="og:image" content="image.jpg">
```

#### og:image:alt

Alt text for the og:image.

```html
<meta property="og:image:alt" content="Alt text for the image">
```

#### og:image:type

MIME type of the og:image.

```html
<meta property="og:image:type" content="image/jpeg">
```

#### og:image:height

Height of the og:image.

```html
<meta property="og:image:height" content="600">
```

#### og:image:width

Width of the og:image.

```html
<meta property="og:image:width" content="800">
```

#### og:site_name

The name of the site or app.

```html
<meta property="og:site_name" content="Site Name">
```

#### og:locale

The locale for the content.

```html
<meta property="og:locale" content="en_US">
```

#### twitter:card

The type of Twitter card to use.

```html
<meta name="twitter:card" content="summary">
```

#### twitter:site

The Twitter handle of the site's creator.

```html
<meta name="twitter:site" content="@username">
```

#### twitter:creator

The Twitter handle of the content creator.

```html
<meta name="twitter:creator" content="@author">
```

> When implementing social media tags, it's important to note that Twitter Card tags (e.g., `twitter:title`, `twitter:description`, etc.) are often unnecessary when equivalent Open Graph tags (e.g., `og:title`, `og:description`, etc.) are present. Twitter will automatically use Open Graph tags as a fallback when generating previews on its platform. Therefore, you can simplify your implementation by focusing on the Open Graph tags and omitting their Twitter Card counterparts. [Twitter Card Fallback Behavior](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started##twitter-cards-and-open-graph)

Learn more: [The Open Graph Protocol](https://ogp.me/), [Facebook Open Graph](https://developers.facebook.com/docs/sharing/webmasters), [Twitter Card Markup](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/markup)

## Extra

Absolutely, let's add information about the `<base>`, `<style>`, `<script>`, and `<noscript>` elements as well:

### Style Tags

Style tags define inline styles directly within the HTML document.

### `<style>`

Defines internal styles for the document.

```html
<style>
  /* Your styles here */
</style>
```

### Script Tags

Script tags are used to include JavaScript code within the HTML document.

#### `<script>`

Includes external or inline JavaScript.

```html
<script src="script.js"></script>
```

### NoScript Tags

NoScript tags provide content for browsers with disabled JavaScript.

#### `<noscript>`

Displays content when JavaScript is disabled.

```html
<noscript>
  <p>Please enable JavaScript to view this site.</p>
</noscript>
```

## 📝 License

This project is licensed under the [MIT License](LICENSE), allowing you to freely use, modify, and distribute the content.