# Working with Docsify

This guide covers how to effectively use Docsify features in your documentation.

## Markdown Basics

Docsify supports standard Markdown syntax plus some extra features:

```markdown
# H1 Heading
## H2 Heading
### H3 Heading

**Bold Text**
*Italic Text*

- Bullet point
- Another point
  - Nested point

1. Numbered list
2. Second item

> Blockquote

`Inline code`

```code
Code block
```

[Link](page.md)
![Image](../images/picture.png)
```

## Special Docsify Features

### 1. Cover Page

Create a `_coverpage.md`:

```markdown
# Document Manager
> A magical documentation site generator.

- Simple and lightweight
- No statically built html files
- Multiple themes

[Get Started](#main)
```

### 2. Sidebar Configuration

In `_sidebar.md`:

```markdown
* [Home](/)
* [Guide](guide.md)
  * [Configuration](configuration.md)
  * [Themes](themes.md)
* [API Reference](api.md)
```

### 3. Navigation Bar

Create `_navbar.md`:

```markdown
* [En](/)
* [中文](/zh-cn/)
```

## Advanced Features

### 1. Adding Plugins

Add to your `index.html`:

```html
<!-- Search -->
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.min.js"></script>

<!-- Copy to Clipboard -->
<script src="//cdn.jsdelivr.net/npm/docsify-copy-code"></script>

<!-- Zoom Image -->
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/zoom-image.min.js"></script>
```

### 2. Custom Styling

Add custom CSS:

```html
<style>
  :root {
    --theme-color: #42b983;
    --sidebar-width: 300px;
  }
</style>
```

### 3. Embedding Content

```markdown
[filename](https://example.js ':include')

<!-- Embedding YouTube -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID"></iframe>
```

## Tips for Documentation

1. **Organization**
   - Keep files organized by topic
   - Use clear, descriptive names
   - Maintain consistent structure

2. **Writing Style**
   - Use clear, concise language
   - Include examples
   - Add screenshots when helpful
   - Keep sections focused

3. **Navigation**
   - Logical menu structure
   - Clear hierarchy
   - Cross-linking related content

4. **Maintenance**
   - Regular updates
   - Check for broken links
   - Update examples
   - Review and revise content

## Troubleshooting

Common issues and solutions:

1. **Sidebar not showing**
   - Check `loadSidebar: true` in config
   - Verify `_sidebar.md` exists
   - Check file permissions

2. **Images not loading**
   - Verify file paths
   - Check image exists
   - Confirm proper syntax

3. **Search not working**
   - Ensure search plugin is loaded
   - Check search configuration
   - Verify content is indexed
