# Claude Code Instructions for HTML/JavaScript Tools Repository

## Repository Purpose
This repository contains a collection of standalone HTML+JavaScript utility tools that will be hosted on a website. Each tool is a separate, self-contained HTML file.

## File Structure and Naming

### Naming Convention
- Each tool must be a single `.html` file
- Use lowercase with hyphens for multi-word names
- Names should be descriptive and clear
- Examples: `timestamp.html`, `color-converter.html`, `json-formatter.html`

### File Organization
- Each tool is completely self-contained in a single `.html` file
- All CSS, JavaScript, and HTML must be included in the same file
- No shared components, libraries, or stylesheets between tools
- No external dependencies required for the tool to function

## Technical Requirements

### JavaScript
- **Prefer vanilla JavaScript** when possible
- Frameworks (React, Vue, etc.) are allowed if the use case justifies them, but should be included via CDN
- All JavaScript must be embedded in `<script>` tags within the HTML file

### CSS and Styling
- All CSS must be embedded in `<style>` tags within the HTML file
- **Mobile-friendly responsive design is required**
- Use responsive units (%, vh, vw, rem, em) and media queries
- Test layouts on mobile, tablet, and desktop screen sizes
- Consider touch-friendly UI elements (larger buttons, adequate spacing)

### HTML Structure
- Use semantic HTML5 elements
- Include proper DOCTYPE, meta tags for viewport and charset
- Each file should be a complete, valid HTML document

## Guidelines for Creating New Tools

### Template Structure
Each tool should follow this basic structure:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Tool Name]</title>
    <style>
        /* All CSS here */
        /* Include responsive design with media queries */
    </style>
</head>
<body>
    <!-- Tool UI here -->

    <script>
        // All JavaScript here
    </script>
</body>
</html>
```

### Best Practices
1. **Self-contained**: Everything needed for the tool must be in the single HTML file
2. **Responsive**: Design mobile-first, then enhance for larger screens
3. **User-friendly**: Clear labels, helpful error messages, intuitive interface
4. **Performance**: Minimize external dependencies, optimize for fast loading
5. **Accessibility**: Use proper ARIA labels, keyboard navigation support where appropriate
6. **Clean code**: Well-organized, commented where necessary
7. **No dependencies**: If using a framework or library, include it via CDN within the file

### When to Use Frameworks
- Default to vanilla JavaScript for simple tools
- Use frameworks when:
  - Complex state management is needed
  - The tool benefits significantly from reactive UI updates
  - The development time would be substantially reduced
- Always include framework via CDN (never external files)

## Testing Checklist
Before considering a tool complete, verify:
- [ ] Works on mobile devices (responsive)
- [ ] Works on tablets
- [ ] Works on desktop
- [ ] All functionality works as expected
- [ ] No console errors
- [ ] File is completely self-contained
- [ ] Code is clean and well-organized
