# Personal Website

A lightweight personal website and blog with minimal dependencies. Perfect for occasional blogging without the complexity of modern frameworks.

## Features

- **Minimal Setup**: Just HTML, CSS, and a tiny bit of JavaScript
- **Public Sans Typography**: Clean, modern font matching professional sites
- **Responsive Design**: Works perfectly on mobile and desktop
- **Semantic HTML**: Proper accessibility with ARIA attributes
- **SEO Ready**: Meta tags for social sharing and search engines
- **Dark Mode**: Automatic support based on system preference
- **Hash Navigation**: Simple article switching with URL support

## Project Structure

```
├── index.html              # Main page with navigation
├── css/styles.css         # Styles with Public Sans font
├── posts/                 # Markdown blog posts
│   ├── first-blog-post.md
│   ├── another-interesting-post.md
│   └── thoughts-on-something-important.md
├── package.json           # Minimal package file (optional)
└── README.md
```

## Getting Started

1. **No installation needed!** Just open `index.html` in a browser

2. **For development server (optional):**
   ```bash
   npm run dev
   ```
   This starts a Python server at http://localhost:8000

3. **Customize content:**
   - Update personal info in `index.html`
   - Change the quote and bio sections
   - Update work history and interests

## Adding New Blog Posts

To add a new article:

1. **Create a new markdown file** in the `posts/` folder:
   ```markdown
   # Your Blog Post Title
   
   *january 15, 2025*
   
   Write your blog post here using markdown. You can use:
   
   - **Bold text**
   - *Italic text*  
   - [Links](https://example.com)
   - Multiple paragraphs
   
   ---
   
   Additional thoughts after a horizontal rule.
   ```

2. **Add a link** in the writing section of `index.html`:
   ```html
   <li><a href="#post/your-file-name" aria-describedby="new-date">Your Blog Post Title</a><span class="date" id="new-date">january 15, 2025</span></li>
   ```

That's it! The JavaScript will automatically load and parse the markdown file.

## Typography

Uses Public Sans font with these specifications:
- **Body text**: Light weight (200), 14px
- **Headings**: Medium weight (500)
- **Links**: Medium weight (500), no underline by default
- **Dates**: Light weight (200), 12px
- **Color**: #191919 (softer than pure black)

## What This Site Avoids

- ❌ Complex JavaScript frameworks
- ❌ Build tools and bundlers
- ❌ External content management systems
- ❌ Multiple file routing
- ❌ Dependencies and package managers

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge).

## License

MIT License - use this template however you like!