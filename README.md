# TEGBot AI Assistant

A modern, interactive AI chat interface built with React.js featuring a sleek design with dark/light theme support, brand colors, and customizable chat background.

![TEGBot Interface](https://img.shields.io/badge/TEGBot-AI%20Assistant-E11E26)

## ✨ Features

- 🤖 **Modern Chat Interface** - Clean and intuitive design with message alignment (bot left, user right)
- 🌓 **Dark/Light Theme Toggle** - Switch between dark and light modes for comfortable viewing
- 🎨 **Brand Colors** - Integrated with #E11E26 (primary red) and #f8f8f9 (light gray)
- 🖼️ **Chat Background Image** - Add your business background image to the chat area
- 💬 **Real-time Messaging** - Instant message sending and receiving
- ⌨️ **Typing Indicators** - Visual feedback when TEGBot is processing
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile
- ⚡ **Fast & Lightweight** - Built with React for optimal performance
- 🔄 **New Chat Option** - Start fresh conversations easily
- ⏰ **Message Timestamps** - Track conversation history
- 🎯 **Smart Message Layout** - Bot messages on left, user messages on right
- 🔍 **Glass-morphism Effects** - Modern blur effects on message bubbles

## 🎨 Brand Integration

### Color Scheme
- **Primary Brand Color**: `#E11E26` (TEG Red)
- **Secondary Brand Color**: `#f8f8f9` (Light Gray)
- Enhanced visual hierarchy with brand colors
- Consistent color usage across both themes

### Chat Background Image
The application supports a custom background image in the chat messages area for a branded conversation experience.

#### To add your chat background:

1. **Add your image to the public folder:**
   ```bash
   # Place your background image in the public folder
   cp your-background.jpg public/chat-background.jpg
   ```
   - Name it `chat-background.jpg`
   - Recommended size: 1920x1080 or higher for best quality
   - Supported formats: .jpg, .jpeg, .png, .webp

2. **The background will automatically:**
   - Display behind the chat messages
   - Have an intelligent overlay for message readability
   - Adapt to dark/light theme changes
   - Scroll with the messages for a seamless experience

3. **If using a different filename:**
   ```css
   /* In src/App.css, update line 226 */
   .messages-container::before {
     background-image: url('/your-custom-name.jpg');
   }
   ```

### Visual Features
- **Chat-specific background** - Background image only in messages area
- **Glass-morphism message bubbles** - Semi-transparent with backdrop blur
- **Dynamic overlays** - Automatic adjustment for readability
- **Theme-adaptive overlays** - Different opacity for dark/light modes
- **Smooth transitions** between themes

## 📋 Prerequisites

Before running this application, ensure you have:

1. **Node.js** (v14 or higher) and npm installed
2. **Backend API** running on `http://localhost:8000` with the `/api/query` endpoint
3. **Chat background image** (optional) for brand customization

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

3. Add your chat background image (optional):
```bash
# Copy your background image to the public folder
cp /path/to/your/background.jpg public/chat-background.jpg
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
│   ├── index.html              # HTML template
│   └── chat-background.jpg     # Your chat background image (add this)
├── src/
│   ├── App.js                  # Main chat component with theme logic
│   ├── App.css                 # Styling with chat background support
│   ├── index.js                # Application entry point
│   └── index.css               # Global styles
├── package.json                # Dependencies and scripts
├── .gitignore                  # Git ignore rules
└── README.md                   # Documentation
```

## 🛠️ Technologies Used

- **React** - Frontend framework
- **Axios** - HTTP client for API calls
- **React Markdown** - Markdown rendering support
- **CSS3** - Modern styling with animations and brand integration

## 🎯 Features in Detail

### Chat Background
- **Localized to chat area** - Background only appears in the messages container
- **Smart overlays** - Automatic overlay adjustment for text readability
- **Theme responsive** - Different overlay opacity for dark (88%) and light (92%) modes
- **Backdrop blur** - Message bubbles have glass effect for better visibility
- **Z-index layering** - Messages appear above background with proper stacking

### Message Styling
- **Glass-morphism effect** - Semi-transparent message bubbles with backdrop blur
- **Brand colors** - User messages in #E11E26, bot messages adapt to theme
- **Enhanced shadows** - Subtle shadows for depth perception
- **Smooth animations** - Fade-in effect for new messages

### Theme System
- **Dark Mode**:
  - Dark overlay (85-90% opacity) over chat background
  - Bot messages: Dark gray with light text
  - Enhanced contrast for readability

- **Light Mode**:
  - Light overlay (88-92% opacity) over chat background
  - Bot messages: Light gray (#f8f8f9) with dark text
  - Softer shadows and colors

## 🎨 Customization Guide

### 1. Chat Background Image
```css
/* Update in src/App.css */
.messages-container::before {
  background-image: url('/chat-background.jpg');
  /* Adjust background properties as needed */
  background-size: cover;  /* or 'contain', '100% 100%' */
  background-position: center;  /* or 'top', 'bottom' */
}
```

### 2. Overlay Opacity
Adjust the overlay darkness/lightness for better readability:
```css
/* Dark theme overlay */
.dark-theme .messages-container::after {
  background: rgba(15, 15, 15, 0.88);  /* Adjust last value (0-1) */
}

/* Light theme overlay */
.light-theme .messages-container::after {
  background: rgba(248, 248, 249, 0.92);  /* Adjust last value (0-1) */
}
```

### 3. Message Bubble Transparency
```css
.message.bot .message-text {
  background: rgba(44, 44, 44, 0.95);  /* Adjust opacity */
  backdrop-filter: blur(20px);  /* Adjust blur amount */
}
```

## 🖼️ Background Image Tips

1. **Image Selection**:
   - Choose images with moderate contrast
   - Avoid busy patterns that might interfere with text
   - Consider abstract or blurred backgrounds

2. **Optimization**:
   - Compress images for web (use tools like TinyPNG)
   - Recommended format: JPEG for photos, PNG for graphics
   - Keep file size under 500KB for best performance

3. **Fallback**:
   - If no image is provided, the chat area uses theme colors
   - Ensures good experience even without custom background

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

**Note**: Remember to include your chat background image in the deployment.

## 🔄 Recent Updates

- ✅ Chat-specific background image (not full app background)
- ✅ Glass-morphism effect on message bubbles
- ✅ Intelligent overlays for readability
- ✅ Theme-adaptive background overlays
- ✅ Enhanced message styling with backdrop blur
- ✅ Z-index layering for proper element stacking

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 💬 Support

For issues or questions, please open an issue on GitHub.

---

**Built with ❤️ by TEGBot Team**