# Quick Setup Guide

This guide will help you get started with Document Manager quickly.

## Directory Structure

Create the following directory structure for your documentation:

```
your-doc-root/
├── docs/
│   ├── README.md
│   ├── _sidebar.md
│   ├── getting-started/
│   ├── usage-guide/
│   └── examples/
└── index.html
```

## Setting Up Docsify

1. Create an `index.html` file in your root directory:

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Document Manager</title>
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/vue.css">
</head>
<body>
  <div id="app"></div>
  <script>
    window.$docsify = {
      name: 'Document Manager',
      repo: '',
      loadSidebar: true,
      subMaxLevel: 3,
      auto2top: true,
      search: {
        maxAge: 86400000,
        paths: 'auto',
        placeholder: 'Type to search',
        noData: 'No Results!',
        depth: 6
      }
    }
  </script>
  <script src="//cdn.jsdelivr.net/npm/docsify/lib/docsify.min.js"></script>
  <script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.min.js"></script>
</body>
</html>
```

## Using Tiny File Manager

1. Access Tiny File Manager at `/tinyfilemanager`
2. Default credentials:
   - Username: admin
   - Password: admin@123
3. Change the default credentials immediately
4. Navigate to your docs directory
5. Start creating and managing your documentation files

## Creating Your First Document

1. Open Tiny File Manager
2. Navigate to your `docs` directory
3. Click "New File"
4. Name it `my-first-doc.md`
5. Add some content:

```markdown
# My First Document

Hello world! This is my first document in Document Manager.

## Section 1

This is a section in my document.

### Subsection

Adding more content here.
```

6. Save the file
7. Add it to your `_sidebar.md`:

```markdown
* [Home](/)
* [My First Document](my-first-doc.md)
```

8. View your documentation through the Docsify interface

## Next Steps

- Explore the [Using Tiny File Manager](../usage-guide/tiny-file-manager.md) guide
- Learn more about [Working with Docsify](../usage-guide/working-with-docsify.md)
- Check out our [Basic Documentation Structure](../examples/basic-structure.md) example
