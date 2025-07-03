# Using Tiny File Manager

This guide explains how to effectively use Tiny File Manager with Docsify for documentation management.

## Basic Operations

### File Management

1. **Creating Files**
   - Click "New File" button
   - Enter filename with `.md` extension
   - Use the built-in editor to write content
   - Click "Save" when done

2. **Creating Directories**
   - Click "New Item" button
   - Select "Directory"
   - Enter directory name
   - Common directories: `images/`, `assets/`, `guides/`

3. **Uploading Files**
   - Click "Upload" button
   - Select files from your computer
   - For images, upload to `images/` directory
   - For other assets, use appropriate directories

### File Organization

Maintain a clean structure:

```
docs/
├── README.md
├── _sidebar.md
├── images/
│   ├── screenshots/
│   └── diagrams/
├── assets/
│   ├── files/
│   └── downloads/
└── content/
    ├── guides/
    ├── tutorials/
    └── reference/
```

## Working with Markdown Files

1. **Editing Files**
   - Click on any `.md` file to open in editor
   - Make changes using Markdown syntax
   - Save changes
   - View instantly in Docsify

2. **Linking Files**
   - Use relative paths in Markdown links
   - Example: `[Link to Guide](../guides/example.md)`
   - For images: `![Image](../images/screenshot.png)`

## Best Practices

1. **File Naming**
   - Use lowercase letters
   - Replace spaces with hyphens
   - Use descriptive names
   - Example: `getting-started-guide.md`

2. **Image Management**
   - Optimize images before upload
   - Use meaningful filenames
   - Organize in subdirectories by topic

3. **Version Control**
   - Download backup regularly
   - Use consistent naming for versions
   - Keep backup copies of important files

## Security Considerations

1. **Access Control**
   - Change default credentials
   - Use strong passwords
   - Regularly update passwords
   - Limit access to authorized users

2. **File Permissions**
   - Set appropriate read/write permissions
   - Restrict sensitive content
   - Regular security audits

## Tips and Tricks

1. **Quick Navigation**
   - Use the search function
   - Bookmark frequently accessed directories
   - Use breadcrumb navigation

2. **Bulk Operations**
   - Select multiple files for operations
   - Use zip/unzip for bulk transfers
   - Batch rename when needed

3. **Troubleshooting**
   - Check file permissions
   - Verify file paths
   - Monitor disk space
   - Check error logs
