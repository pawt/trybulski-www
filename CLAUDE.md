# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a lightweight personal website and blog with minimal dependencies. Perfect for someone who writes one blog post per month and wants to keep things simple.

## Architecture

- **Simple Structure**: Just HTML and CSS with minimal inline JavaScript
- **External Stylesheet**: `css/styles.css` with Public Sans typography
- **Inline JavaScript**: Basic navigation logic embedded in HTML
- **Single File Articles**: Articles are sections within the main HTML file
- **No Build Process**: Just open `index.html` or use a simple dev server

## Development Commands

- `npm run dev` - Start Python development server on port 8000
- `npm start` - Same as dev command

## File Structure
```
├── index.html              # Main page with navigation
├── css/styles.css         # Styles with Public Sans font
├── posts/                 # Markdown blog posts
│   ├── first-blog-post.md
│   ├── another-interesting-post.md
│   └── thoughts-on-something-important.md
├── package.json           # Minimal package file
└── README.md              # Documentation
```

## Key Features

- **Public Sans Typography**: Matches catherinejue.com styling
- **Responsive Design**: Mobile-first with 600px breakpoint  
- **Semantic HTML**: Proper markup with ARIA labels
- **Hash Navigation**: Simple article switching with URL support
- **Dark Mode Support**: Automatic based on system preference
- **SEO Ready**: Meta tags for social sharing

## Adding New Blog Posts

To add a new blog post:

1. **Create a new markdown file** in the `posts/` folder:
   ```markdown
   # Your Blog Post Title
   
   *january 15, 2025*
   
   Your blog content here. You can use **bold**, *italic*, and [links](https://example.com).
   
   Use multiple paragraphs as needed.
   
   ---
   
   Additional notes after a separator.
   ```

2. **Add a link** to the writing section in `index.html`:
   ```html
   <li><a href="#post/your-file-name" aria-describedby="new-date">Your Blog Post Title</a><span class="date" id="new-date">january 15, 2025</span></li>
   ```

The JavaScript will automatically load and parse the markdown file when clicked.

## Typography

Uses Public Sans font with these specifications:
- **Body**: 200 weight, 14px, -0.25px letter-spacing
- **Headings**: 500 weight  
- **Links**: 500 weight, no underline by default
- **Dates**: 200 weight, 12px
- **Color**: #191919 (softer than pure black)

## No Build Tools Needed

This site intentionally avoids:
- ❌ Complex JavaScript frameworks
- ❌ Build processes or bundlers  
- ❌ Linting tools or configs
- ❌ External content management
- ❌ Multiple file routing

Perfect for a simple personal blog updated monthly!