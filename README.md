# TEGBot AI Assistant

A modern, interactive AI chat interface built with React.js featuring a sleek design with dark/light theme support, brand colors, and customizable background imagery.

![TEGBot Interface](https://img.shields.io/badge/TEGBot-AI%20Assistant-E11E26)

## ✨ Features

- 🤖 **Modern Chat Interface** - Clean and intuitive design with message alignment (bot left, user right)
- 🌓 **Dark/Light Theme Toggle** - Switch between dark and light modes for comfortable viewing
- 🎨 **Brand Colors** - Integrated with #E11E26 (primary red) and #f8f8f9 (light gray)
- 🖼️ **Background Image Support** - Add your business background image for branding
- 💬 **Real-time Messaging** - Instant message sending and receiving
- ⌨️ **Typing Indicators** - Visual feedback when TEGBot is processing
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile
- ⚡ **Fast & Lightweight** - Built with React for optimal performance
- 🔄 **New Chat Option** - Start fresh conversations easily
- ⏰ **Message Timestamps** - Track conversation history
- 🎯 **Smart Message Layout** - Bot messages on left, user messages on right

## 🎨 Brand Integration

### Color Scheme
- **Primary Brand Color**: `#E11E26` (TEG Red)
- **Secondary Brand Color**: `#f8f8f9` (Light Gray)
- Enhanced visual hierarchy with brand colors
- Consistent color usage across both themes

### Background Image Setup
The application supports a custom background image to reinforce your brand identity.

#### To add your background image:

1. **Add your image to the public folder:**
   - Place your background image in the `public` folder
   - Name it `background.jpg` (or update the CSS with your filename)
   - Recommended size: 1920x1080 or higher for best quality

2. **Optional: Add a chat pattern texture:**
   - Add a subtle pattern image to `public/chat-pattern.png`
   - This will overlay on the messages area for texture

3. **Update the CSS if using different filenames:**
   ```css
   /* In src/App.css, update the background-image URL */
   .app::before {
     background-image: url('/your-background-image.jpg');
   }
   ```

### Visual Features
- **Glass-morphism effects** with backdrop filters
- **Gradient overlays** for better text readability
- **Dynamic shadows** using brand colors
- **Smooth transitions** between themes

## 📋 Prerequisites

Before running this application, ensure you have:

1. **Node.js** (v14 or higher) and npm installed
2. **Backend API** running on `http://localhost:8000` with the `/api/query` endpoint
3. **Background image** (optional) for brand customization

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

3. Add your background image (optional):
```bash
# Copy your background image to the public folder
cp /path/to/your/background.jpg public/background.jpg
```

4. Start the development server:
```bash
npm start
```

5. Open your browser and navigate to:
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
│   ├── index.html          # HTML template
│   ├── background.jpg      # Your brand background image (add this)
│   └── chat-pattern.png    # Optional texture overlay (add this)
├── src/
│   ├── App.js             # Main chat component with theme logic
│   ├── App.css            # Styling with brand colors and background
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
- **CSS3** - Modern styling with animations and brand integration

## 🎯 Features in Detail

### Brand Integration
- **Color Usage**: #E11E26 for primary actions and accents, #f8f8f9 for light backgrounds
- **Background Image**: Full-screen background with intelligent overlays
- **Glass Effects**: Modern glassmorphism for a premium feel
- **Dynamic Theming**: Colors adapt beautifully in both dark and light modes

### Chat Interface
- Clean, modern design with brand colors
- Message bubbles with distinct left/right alignment
- Bot messages appear on the left with subtle brand coloring
- User messages appear on the right with primary brand color
- Smooth scrolling and animations
- Markdown support for formatted responses

### Theme System
- Toggle between dark and light modes
- Brand colors integrated in both themes
- Background image adapts to theme with overlays
- Smooth transitions between themes

## 🎨 Customization Guide

### 1. Background Image
```css
/* Update in src/App.css */
.app::before {
  background-image: url('/your-custom-background.jpg');
}
```

### 2. Brand Colors
```css
/* Update the root variables in src/App.css */
:root {
  --brand-primary: #E11E26;    /* Your primary color */
  --brand-secondary: #f8f8f9;  /* Your secondary color */
}
```

### 3. Chat Bubble Colors
- User messages use the primary brand color (#E11E26)
- Bot messages use the secondary color (#f8f8f9) in light mode
- All colors are optimized for readability

### 4. Additional Customization
- Modify overlay opacity for background image visibility
- Adjust blur effects for glassmorphism
- Change gradient directions and colors
- Update shadow colors to match your brand

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

**Note**: Remember to include your background images in the deployment.

## 🔄 Recent Updates

- ✅ Integrated brand colors #E11E26 and #f8f8f9 throughout the interface
- ✅ Added background image support with intelligent overlays
- ✅ Enhanced visual design with glassmorphism effects
- ✅ Improved color consistency across themes
- ✅ Added gradient overlays for better readability
- ✅ Implemented dynamic shadows using brand colors

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 💬 Support

For issues or questions, please open an issue on GitHub.

---

**Built with ❤️ by TEGBot Team**