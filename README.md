# markdown-to-html-test01

## Overview
A production-ready single-page application that converts Markdown content to HTML using the marked.js library and applies syntax highlighting to code blocks using highlight.js. The application processes the provided `input.md` file and renders it beautifully with modern styling.

## Features
- **Markdown Parsing**: Converts Markdown to HTML using marked.js library
- **Syntax Highlighting**: Automatically highlights code blocks using highlight.js
- **Responsive Design**: Built with Bootstrap 5 for mobile-friendly layouts
- **Modern UI**: Gradient backgrounds and card-based layout
- **Self-Contained**: No server required - runs entirely in the browser
- **Error Handling**: Graceful error handling with user feedback
- **Production Ready**: Clean, well-commented code with proper structure

## Setup Instructions
1. Clone the repository
2. Open index.html in a web browser
3. The application runs entirely client-side

No build process, dependencies, or server required!

## Usage
Simply open the `index.html` file in any modern web browser. The application will automatically:
1. Load the markdown content from the embedded `input.md` data
2. Parse the markdown using marked.js
3. Render the HTML output in the `#markdown-output` div
4. Apply syntax highlighting to all code blocks
5. Display a success status indicator

The rendered output includes:
- Properly formatted headings
- Styled lists with custom bullets
- Syntax-highlighted code blocks
- Responsive typography

## Code Explanation
The application works through the following process:

1. **Library Loading**: Loads marked.js (v11.1.1) and highlight.js (v11.9.0) from CDN
2. **Content Embedding**: The markdown content from `input.md` is embedded directly in the HTML as a JavaScript string
3. **Configuration**: Marked.js is configured with custom options including highlight.js integration
4. **Conversion**: The `marked.parse()` function converts markdown to HTML
5. **Rendering**: The HTML is injected into the `#markdown-output` div
6. **Highlighting**: highlight.js processes all code blocks for syntax highlighting
7. **Verification**: The app verifies all libraries loaded correctly before initialization

## Technologies Used
- **marked.js** (v11.1.1) - Markdown parser and compiler
- **highlight.js** (v11.9.0) - Syntax highlighting for code blocks
- **Bootstrap** (v5.3.2) - CSS framework for responsive design
- **Vanilla JavaScript** - No additional frameworks required
- **CSS3** - Modern styling with gradients and animations

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