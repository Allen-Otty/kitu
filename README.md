# AI Code Editor

An AI-powered application with ChatGPT-like interface that can chat with users and edit its own code according to instructions.

## Features

- 🤖 **AI Chat Interface**: ChatGPT-like conversational interface
- 📝 **Code Editing**: AI can create, modify, and delete files in the project
- 🔄 **Real-time Updates**: Apply code changes directly from the chat interface
- 📁 **File Management**: Browse, read, and manage project files
- 🎨 **Modern UI**: Clean, responsive interface similar to ChatGPT

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the backend server:
```bash
npm run server
```

3. In a new terminal, start the frontend development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

## Usage

### Chat with AI
- Type messages in the chat input at the bottom
- The AI will respond with helpful information and code suggestions
- Ask the AI to create components, modify files, or explain code

### Code Editing Features
- Ask the AI to "create a new component"
- Request modifications to existing files
- The AI will show code changes with an "Apply Changes" button
- Click the button to save changes directly to your project files

### Example Prompts
- "Create a new React component called UserProfile"
- "Modify the App.jsx file to add a counter"
- "Add some CSS styling to make the buttons look better"
- "Create a utility function for formatting dates"

## API Endpoints

The backend provides several endpoints for file operations:

- `POST /api/edit-file` - Create or modify files
- `GET /api/read-file` - Read file contents
- `GET /api/list-files` - List files in a directory
- `DELETE /api/delete-file` - Delete files
- `GET /api/health` - Health check

## Project Structure

```
ai-code-editor/
├── src/
│   ├── App.jsx          # Main React component
│   ├── main.jsx         # React entry point
│   └── index.css        # Styles
├── server/
│   └── index.js         # Express backend
├── package.json         # Dependencies and scripts
├── vite.config.js       # Vite configuration
└── README.md           # This file
```

## Security

- File operations are restricted to the project directory
- Path traversal attacks are prevented
- File size limits are enforced

## Development

To extend the application:

1. **Add new AI capabilities**: Modify the `simulateAIResponse` function in `App.jsx`
2. **Add new API endpoints**: Extend the Express server in `server/index.js`
3. **Customize UI**: Modify the CSS in `src/index.css`
4. **Add real AI integration**: Replace the mock AI responses with actual AI API calls

## Technologies Used

- **Frontend**: React, Vite, Axios
- **Backend**: Node.js, Express
- **Styling**: CSS3 with ChatGPT-inspired design
- **File System**: Node.js fs/promises for file operations

## License

MIT License - feel free to use this project as a starting point for your own AI-powered applications!