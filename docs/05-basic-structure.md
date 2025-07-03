# Basic Documentation Structure Example

This example demonstrates how to organize a basic documentation project using Document Manager.

## Project: API Documentation Example

Here's a complete example of how to structure API documentation:

### Directory Structure

```
docs/
├── README.md
├── _sidebar.md
├── api/
│   ├── authentication.md
│   ├── endpoints.md
│   └── errors.md
├── guides/
│   ├── getting-started.md
│   └── best-practices.md
└── images/
    └── diagrams/
        └── api-flow.png
```

### Example Content

#### README.md
```markdown
# API Documentation

Welcome to our API documentation. This guide will help you integrate with our service.

## Quick Links
- [Authentication](api/authentication.md)
- [API Endpoints](api/endpoints.md)
- [Error Handling](api/errors.md)
```

#### _sidebar.md
```markdown
* [Home](/)
* API Reference
  * [Authentication](api/authentication.md)
  * [Endpoints](api/endpoints.md)
  * [Errors](api/errors.md)
* Guides
  * [Getting Started](guides/getting-started.md)
  * [Best Practices](guides/best-practices.md)
```

### Live Example: Authentication Documentation

Here's how the authentication.md file might look:

```markdown
# Authentication

## Overview
Our API uses JWT (JSON Web Tokens) for authentication.

## Getting Started
1. Register for an API key
2. Include the key in your requests
3. Handle the JWT token in responses

## Code Example
```javascript
fetch('https://api.example.com/auth', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json',
    'X-API-Key': 'your-api-key'
  },
  body: JSON.stringify({
    username: 'user',
    password: 'pass'
  })
})
```

## Managing Files with Tiny File Manager

1. Create the directory structure:
   - Use "New Item" to create directories
   - Create each .md file
   - Upload any images to the images directory

2. Edit files:
   - Use the built-in editor
   - Preview changes in Docsify
   - Maintain consistent formatting

3. Organize content:
   - Group related files in directories
   - Use clear file names
   - Keep image assets separate
