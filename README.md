# PromptPilot-AI

A powerful browser extension that enhances your AI prompting experience with intelligent features and seamless integration.

## Features

- 🚀 Smart prompt management
- 🤖 AI-powered assistance
- 💾 Save and organize prompts
- ⚡ Quick access to frequently used prompts
- 🎯 Real-time AI integration
- 📝 Context-aware suggestions

## Project Structure

```
├── src/
│   ├── App.jsx           # Main React component
│   ├── background.js     # Extension background script
│   ├── content.js        # Content script for webpage integration
│   ├── main.jsx          # React entry point
│   └── index.css         # Styles
├── public/
│   └── icons/           # Extension icons (16x16, 48x48, 128x128)
├── index.html           # Main HTML file
├── manifest.json        # Extension manifest
├── package.json         # Project dependencies
├── vite.config.js       # Vite configuration
└── README.md           # This file
```

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Modern web browser (Chrome, Edge, Firefox)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Bindu2020324/PromptPilot-AI.git
   cd PromptPilot-AI
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Build the project**
   ```bash
   npm run build
   ```

## Running from a shared ZIP

If you send someone the ZIP file, they must follow these steps:

1. unzip the project folder
2. open a terminal in the project folder
3. run `npm install`
4. run `npm run build`
5. load the extension from the generated `dist/` folder in the browser

### If you want the ZIP to work without requiring npm install

1. build the project locally first:
   ```bash
   npm install
   npm run build
   ```
2. include the entire `dist/` folder in the ZIP
3. the recipient can then load the unpacked extension directly from `dist/`

### Loading the built extension

1. Open your browser extension page:
   - Chrome/Edge: `chrome://extensions/`
   - Firefox: `about:debugging#/runtime/this-firefox`
2. Enable **Developer Mode** (Chrome/Edge)
3. Click **Load unpacked** and choose the `dist/` folder

### Free GitHub-built version

If your repository is public, this project automatically builds on every push to `main` and uploads a ready-to-download `dist` artifact.

To use it:

1. Open your repository on GitHub
2. Go to **Actions**
3. Open the latest `Build and package extension` workflow run
4. Download the `promptpilot-ai-dist` artifact
5. Unzip and load the `dist/` folder as an unpacked extension

This gives users a simple free way to try the extension without running `npm install` or `npm run build` themselves.

## Development

### Running in Development Mode

```bash
npm run dev
```

This will start the Vite development server and watch for changes.

### Loading the Extension

1. Open your browser and go to the extensions page:
   - **Chrome/Edge**: `chrome://extensions/` or `edge://extensions/`
   - **Firefox**: `about:debugging#/runtime/this-firefox`

2. Enable **Developer Mode** (top-right corner for Chrome/Edge)

3. Click **Load unpacked** and select the `dist` folder from your project

## Building

```bash
npm run build
```

This creates an optimized build in the `dist` folder ready for distribution.

## Configuration

Edit `manifest.json` to customize:
- Extension name and description
- Permissions
- Icons and branding
- Content scripts and background behavior

## Technologies Used

- **React** - UI framework
- **Vite** - Build tool
- **JavaScript** - Core logic
- **CSS** - Styling

## File Descriptions

| File | Purpose |
|------|---------|
| `manifest.json` | Defines extension metadata and permissions |
| `background.js` | Handles background tasks and extension logic |
| `content.js` | Injects functionality into web pages |
| `App.jsx` | Main React component |
| `vite.config.js` | Build configuration |

## Contributing

Contributions are welcome! Please feel free to submit issues and enhancement requests.

See [CONTRIBUTING.md](CONTRIBUTING.md) for local setup, branch naming, PR checklist, and testing instructions.

## License

MIT License - see LICENSE file for details

## Support

For questions or issues, please open an issue on [GitHub](https://github.com/Bindu2020324/PromptPilot-AI/issues).

---

**Built with ❤️ using React and Vite**