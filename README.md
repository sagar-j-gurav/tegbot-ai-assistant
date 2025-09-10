# TEGBot AI Assistant

A modern, interactive AI chat interface built with React.js featuring a sleek design with dark/light theme support and real-time conversation capabilities.

![TEGBot Interface](https://img.shields.io/badge/TEGBot-AI%20Assistant-E11E26)

## ✨ Features

- 🤖 **Modern Chat Interface** - Clean and intuitive design with message alignment (bot left, user right)
- 🌓 **Dark/Light Theme Toggle** - Switch between dark and light modes for comfortable viewing
- 💬 **Real-time Messaging** - Instant message sending and receiving
- ⌨️ **Typing Indicators** - Visual feedback when TEGBot is processing
- 🎨 **Custom Branding** - TEGBot themed with primary color #E11E26
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile
- ⚡ **Fast & Lightweight** - Built with React for optimal performance
- 🔄 **New Chat Option** - Start fresh conversations easily
- ⏰ **Message Timestamps** - Track conversation history
- 🎯 **Smart Message Layout** - Bot messages on left, user messages on right

## 🎨 Theme Features

### Dark Mode
- Rich dark backgrounds with high contrast
- Easy on the eyes for extended use
- Vibrant accent colors

### Light Mode
- Clean, bright interface
- Professional appearance
- Soft shadows and subtle gradients

## 📋 Prerequisites

Before running this application, ensure you have:

1. **Node.js** (v14 or higher) and npm installed
2. **Backend API** running on `http://localhost:8000` with the `/api/query` endpoint

## 🚀 Installation

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

## 🔧 Backend API Setup

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

## 📁 Project Structure

```
tegbot-ai-assistant/
├── public/
│   └── index.html          # HTML template
├── src/
│   ├── App.js             # Main chat component with theme logic
│   ├── App.css            # Styling with dark/light theme support
│   ├── index.js           # Application entry point
│   └── index.css          # Global styles
├── package.json           # Dependencies and scripts
├── .gitignore            # Git ignore rules
└── README.md             # Documentation
```

## 🛠️ Technologies Used

- **React** - Frontend framework
- **Axios** - HTTP client for API calls
- **React Markdown** - Markdown rendering support
- **CSS3** - Modern styling with animations and theme variables

## 🎯 Features in Detail

### Chat Interface
- Clean, modern design with theme support
- Message bubbles with distinct left/right alignment
- Bot messages appear on the left side
- User messages appear on the right side
- Smooth scrolling and animations
- Markdown support for formatted responses

### Theme System
- Toggle between dark and light modes
- Smooth transitions between themes
- Persistent theme preference (can be enhanced with localStorage)
- Optimized color schemes for both modes

### Typing Indicator
- Animated dots showing when TEGBot is thinking
- Provides visual feedback during API calls

### Error Handling
- Graceful error messages when API is unavailable
- Connection status indicators
- User-friendly error displays

### Responsive Design
- Adapts to different screen sizes
- Mobile-friendly touch interactions
- Optimized layout for both desktop and mobile

## 🎨 Customization

You can customize TEGBot by modifying:

1. **Colors**: Edit CSS variables in `src/App.css` for both themes
2. **API Endpoint**: Update the URL in `src/App.js`
3. **Bot Messages**: Customize welcome and error messages
4. **Theme Defaults**: Change initial theme preference in `App.js`
5. **Styling**: Modify the theme and layout in CSS files

## 📦 Building for Production

To create a production build:

```bash
npm run build
```

This will create an optimized build in the `build/` directory.

## 🚀 Deployment

The production build can be deployed to:
- Netlify
- Vercel
- GitHub Pages
- Any static hosting service

## 🔄 Recent Updates

- ✅ Added left/right message alignment (bot left, user right)
- ✅ Implemented dark/light theme toggle
- ✅ Enhanced visual design for both themes
- ✅ Improved message bubble styling
- ✅ Added theme-specific color schemes

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 💬 Support

For issues or questions, please open an issue on GitHub.

---

**Built with ❤️ by TEGBot Team**