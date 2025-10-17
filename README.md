# markdown-to-html-test01

## Overview
A modern, single-page web application that displays Markdown content with an interactive tabbed interface. Users can seamlessly switch between viewing the rendered HTML output and the original Markdown source code. The application is fully client-side and requires no server setup.

## Features
- **Dual View Modes**: Toggle between beautifully rendered HTML and raw Markdown source
- **Syntax Highlighting**: Code blocks are automatically highlighted using Highlight.js
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, gradient-based design with smooth animations
- **Zero Dependencies**: Runs entirely in the browser with no backend required
- **GitHub Flavored Markdown**: Full support for GFM syntax including tables, task lists, and more
- **Instant Rendering**: Fast, client-side Markdown parsing with Marked.js

## Setup Instructions
1. Clone the repository
   bash
   git clone https://github.com/yourusername/markdown-to-html-test01.git
   
2. Open index.html in a web browser
3. The application runs entirely client-side - no build process or server required

## Usage
1. **Open the Application**: Simply open `index.html` in any modern web browser
2. **View Rendered HTML**: The default view shows the Markdown rendered as styled HTML with syntax-highlighted code blocks
3. **View Source**: Click the "📄 Markdown Source" tab to see the original Markdown text
4. **Switch Between Views**: Click either tab to toggle between rendered and source views
5. **Content Sync**: Both views display the same content - changes to the source would be reflected in both tabs

## Code Explanation

### Core Components
- **Markdown Parsing**: Uses Marked.js library to convert Markdown to HTML
- **Syntax Highlighting**: Highlight.js provides beautiful code syntax highlighting
- **Tab System**: Custom JavaScript implementation for smooth tab switching
- **Responsive Layout**: Bootstrap 5 provides the responsive grid and utilities

### Key Functions
- `renderMarkdown()`: Parses the Markdown content and populates both the rendered HTML and source views
- `setupTabs()`: Initializes the tab switching functionality with event listeners
- `marked.setOptions()`: Configures Marked.js to integrate with Highlight.js for code highlighting

### Data Flow
1. Markdown content is stored as a JavaScript string constant
2. On page load, the content is parsed by Marked.js
3. Rendered HTML is injected into `#markdown-output`
4. Original text is displayed in `#markdown-source`
5. Tab buttons control visibility of each view

## Technologies Used
- **HTML5**: Semantic markup and structure
- **CSS3**: Custom styling with gradients, animations, and flexbox
- **JavaScript (ES6+)**: Modern JavaScript for DOM manipulation and event handling
- **Bootstrap 5.3.0**: Responsive layout and utility classes
- **Marked.js 9.1.0**: Fast Markdown parser and compiler
- **Highlight.js 11.8.0**: Syntax highlighting for code blocks

## License
MIT License

Copyright (c) 2024

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.