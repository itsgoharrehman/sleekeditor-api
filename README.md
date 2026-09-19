# sleekeditor-api

A modern, dependency-free, and offline-first custom rich-text WYSIWYG editor component. Exposes a clean, object-oriented JavaScript Class API with real-time word/character telemetry, block formatting presets, customizable toolbars, and dynamic theme switching.

## Architecture and Stack

* **Language**: Vanilla JavaScript (ES6+ Class Architecture)
* **Styling**: Vanilla CSS3 custom properties (design tokens)
* **Core API**: Native DOM `contenteditable`, Selection API, and Range API
* **Bundle Footprint**: Sub-15KB unminified, zero external NPM dependencies

## Key Features

* **Class-Based Instantiation**: Embed multiple isolated editor instances on a single page with custom selector bindings.
* **Block & Inline Formatting**: Headings (H1-H6), quotes, code snippets, lists, bold, italics, underline, and links.
* **Real-Time Analytics**: Built-in event hooks for word count, character count, and estimated reading time.
* **Theme System**: Seamless dark and light mode adaptation via CSS variables.

## Getting Started

### Installation
```bash
git clone https://github.com/itsgoharrehman/sleekeditor-api.git
cd sleekeditor-api
```

### Usage
```html
<link rel="stylesheet" href="sleekeditor.css">
<div id="editor-container"></div>
<script src="sleekeditor.js"></script>
<script>
  const editor = new SleekEditor('#editor-container', {
    placeholder: 'Write your content here...',
    theme: 'dark',
    toolbar: ['bold', 'italic', 'heading', 'link', 'list', 'code']
  });
</script>
```

## API Reference

* `editor.getContent()`: Returns serialized HTML string.
* `editor.getText()`: Returns raw plain-text content.
* `editor.setContent(html)`: Loads markup into the editor instance.
* `editor.clear()`: Resets editor to empty state.

## Security Policy

Report vulnerabilities to `goharrehmanfsd260@gmail.com`.

## Maintainer

* **Gohar Rehman**
* GitHub: [@itsgoharrehman](https://github.com/itsgoharrehman)
* Email: `goharrehmanfsd260@gmail.com`
* Website: [itsgoharrehman.netlify.app](https://itsgoharrehman.netlify.app/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
