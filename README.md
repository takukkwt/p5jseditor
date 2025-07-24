# p5.js Local Editor

A complete local development environment for p5.js creative coding. This editor runs entirely in your browser without requiring any external connections, making it perfect for offline development and educational environments.

## ✨ Features

### Core Editor
- **Monaco Editor Integration**: Full-featured code editor with syntax highlighting
- **Real-time Preview**: Instant code execution with live canvas updates
- **Error Detection**: Built-in error checking and display
- **Auto-completion**: p5.js function suggestions and JavaScript ES6+ support
- **Console Output**: Built-in console for debugging and logging

### File Management
- **Local File Access**: Open and save files directly from your computer (modern browsers)
- **Project Management**: Organize multiple files and projects
- **Auto-save**: Automatic saving with configurable intervals
- **Recent Files**: Quick access to recently opened files
- **Export Options**: Export projects as standalone HTML files

### User Interface
- **Dark/Light Theme**: Toggle between themes
- **Responsive Design**: Works on desktop and mobile devices
- **Customizable Layout**: Resizable panels and configurable settings
- **p5.js Reference**: Built-in function reference with search
- **Settings Panel**: Comprehensive configuration options

### Advanced Features
- **Multiple File Support**: Work with multiple sketches simultaneously
- **File System Integration**: Direct file system access (where supported)
- **Performance Monitoring**: Built-in performance metrics
- **Keyboard Shortcuts**: Efficient workflow with hotkeys

## 🚀 Getting Started

### Option 1: Use the Built Version (Recommended)
1. Download the `dist` folder from this repository
2. Open `index.html` in a modern web browser
3. Start coding with p5.js!

### Option 2: Development Setup
1. Clone this repository
2. Install dependencies: `pnpm install`
3. Start development server: `pnpm run dev`
4. Open http://localhost:5173 in your browser

## 📁 Project Structure

```
p5js-local-editor/
├── dist/                 # Built files (ready to use)
├── src/
│   ├── components/       # React components
│   ├── store/           # State management
│   ├── utils/           # Utility functions
│   └── App.jsx          # Main application
├── public/              # Static assets
└── package.json         # Dependencies
```

## 🎯 Usage

### Creating Your First Sketch
1. Click "Create New File" or use the "+" button
2. Write your p5.js code in the editor
3. Click "Run" to see your sketch in the preview panel
4. Use the console to debug your code

### File Operations
- **Open File**: Load .js files from your computer
- **Save File**: Save your work locally
- **Export HTML**: Create a standalone HTML file with your sketch
- **Auto-save**: Automatically saves your work every 10 seconds (configurable)

### Customization
- Access settings through the sidebar
- Adjust editor preferences (font size, theme, etc.)
- Configure auto-save intervals
- Customize preview settings

## 🔧 Browser Compatibility

### Fully Supported Features
- Chrome 86+
- Edge 86+
- Firefox 82+
- Safari 14+

### File System Access
Modern browsers support direct file system access. Older browsers will use download/upload fallbacks.

## 📝 Keyboard Shortcuts

- `Ctrl/Cmd + Enter`: Run code
- `Ctrl/Cmd + S`: Save file
- `Ctrl/Cmd + N`: New file
- `Ctrl/Cmd + O`: Open file
- `Ctrl/Cmd + \``: Toggle console

## 🎨 Example Sketches

### Basic Animation
```javascript
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  
  // Draw a circle that follows the mouse
  fill(255, 0, 100);
  ellipse(mouseX, mouseY, 50, 50);
}
```

### Interactive Drawing
```javascript
function setup() {
  createCanvas(800, 600);
  background(255);
}

function draw() {
  if (mouseIsPressed) {
    stroke(random(255), random(255), random(255));
    strokeWeight(random(1, 10));
    line(mouseX, mouseY, pmouseX, pmouseY);
  }
}
```

## 🛠️ Development

### Building from Source
```bash
# Install dependencies
pnpm install

# Start development server
pnpm run dev

# Build for production
pnpm run build

# Preview production build
pnpm run preview
```

### Technologies Used
- **React 18**: UI framework
- **Monaco Editor**: Code editor
- **Zustand**: State management
- **Tailwind CSS**: Styling
- **Vite**: Build tool
- **p5.js**: Creative coding library

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

## 🔗 Related Projects

- [p5.js](https://p5js.org/) - The creative coding library this editor supports
- [Monaco Editor](https://microsoft.github.io/monaco-editor/) - The code editor component
- [OpenProcessing](https://openprocessing.org/) - Online p5.js community

## 📞 Support

If you encounter any issues or have questions:
1. Check the browser console for error messages
2. Ensure you're using a modern browser
3. Try refreshing the page
4. For file access issues, check browser permissions

---

**Happy Creative Coding! 🎨**

