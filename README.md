# TEGBot AI Assistant

A modern, interactive AI chat interface built with React.js featuring a sleek dark theme and real-time conversation capabilities.

![TEGBot Interface](https://img.shields.io/badge/TEGBot-AI%20Assistant-E11E26)

## Features

- 🤖 **Modern Chat Interface** - Clean and intuitive design with dark theme
- 💬 **Real-time Messaging** - Instant message sending and receiving
- ⌨️ **Typing Indicators** - Visual feedback when TEGBot is processing
- 🎨 **Custom Branding** - TEGBot themed with primary color #E11E26
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile
- ⚡ **Fast & Lightweight** - Built with React for optimal performance
- 🔄 **New Chat Option** - Start fresh conversations easily
- ⏰ **Message Timestamps** - Track conversation history

## Prerequisites

Before running this application, ensure you have:

1. **Node.js** (v14 or higher) and npm installed
2. **Backend API** running on `http://localhost:8000` with the `/api/query` endpoint

## Installation

1. Clone the repository:
```bash
git clone https://github.com/sagar-j-gurav/tegbot-ai-assistant.git
cd tegbot-ai-assistant
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

4. Open your browser and navigate to:
```
http://localhost:3000
```

## Backend API Setup

Ensure your backend API is running with the following endpoint:

- **Endpoint**: `POST http://localhost:8000/api/query`
- **Request Body**:
```json
{
  "query": "Your message here"
}
```
- **Response**:
```json
{
  "answer": "Bot response here"
}
```

## Technologies Used

- **React** - Frontend framework
- **Axios** - HTTP client for API calls
- **React Markdown** - Markdown rendering support
- **CSS3** - Modern styling with animations

## License

This project is open source and available under the MIT License.

---

**Built with ❤️ by TEGBot Team**