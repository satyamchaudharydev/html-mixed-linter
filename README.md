# html-mixed-linter

A linter for HTML code with embedded CSS and JavaScript.

## Installation
npm install html-mixed-linter

## Usage

### Integrating with CodeMirror

To integrate `html-mixed-linter` with CodeMirror, follow these steps:

1. Import the necessary modules in your JavaScript file:

```javascript
import { htmlLinter, cssLinter, jsLinter } from 'html-mixed-linter';
const editor = new EditorView({
  extensions: [
    // ... other extensions ...
    linter(htmlLinter),
    linter(cssLinter),
    linter(jsLinter)
  ],
  // ... other configurations ...
});

Start writing your HTML code with embedded CSS and JavaScript in the CodeMirror editor. Any linting errors or warnings will be displayed.