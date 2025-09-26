# Google Chat Takeout Viewer

A modern, **single-file web application** for viewing Google Chat message history from Google Takeout exports. Experience your chat history with a clean, Google Chat-like interface that works entirely in your browser.

![Google Chat Takeout Viewer](https://img.shields.io/badge/Type-Single%20File%20Web%20App-blue) ![Browser Support](https://img.shields.io/badge/Browser-Chrome%2FEdge%2FSafari-green) ![No Server Required](https://img.shields.io/badge/Server-Not%20Required-brightgreen)

## ✨ Features

### 🎨 **Modern Google Chat Interface**
- **Authentic Design**: Pixel-perfect recreation of Google Chat's interface
- **Material Design**: Uses Google's official design tokens and typography
- **Responsive Layout**: Works seamlessly on desktop, tablet, and mobile devices
- **Dark Mode Ready**: Clean, modern styling that's easy on the eyes

### 💬 **Rich Chat Experience**
- **Message Bubbles**: Individual message cards with avatars and timestamps  
- **Right-Aligned Messages**: Your messages appear on the right (like WhatsApp/iMessage)
- **Smart Avatars**: Dynamic initials and colors, emoji avatars for Spaces
- **Message Reactions**: Display emoji reactions and interactions
- **Hyperlink Processing**: Automatic link detection with rich previews

### 🔍 **Powerful Search**
- **Dual Search System**: 
  - **Chat Search**: Find chats by name or member names
  - **Message Search**: Search within messages with highlighting (fixed in header)
- **Real-time Filtering**: Instant results as you type
- **Member-based Discovery**: Find chats by participant names

### 📁 **Smart Organization**
- **Grouped Sidebar**: Organized into Direct Messages and Spaces
- **Collapsible Sections**: Clean, manageable chat organization
- **Member Count Display**: Click to see all chat participants
- **Activity Status**: Visual indicators for active/selected chats

### 🎵 **Rich Media Support**
- **Image Galleries**: Thumbnail previews with click-to-expand modal
- **Audio Players**: Built-in audio controls for voice messages
- **File Attachments**: Support for documents, archives, and other file types
- **Modal Image Viewer**: Full-screen image viewing with keyboard shortcuts

### ⚡ **Advanced Features**
- **Message Pagination**: Handle large chat histories (5000+ messages)
- **Jump to Message**: Direct navigation to specific message numbers
- **Filter Options**: Show only images, hide specific members
- **Export-Friendly**: No server required, works with any Google Takeout export

## 🚀 Getting Started

### Prerequisites
- **Modern Browser**: Chrome 86+, Edge 86+, or Safari 14+ (requires File System Access API)
- **Google Takeout Export**: Download your Google Chat data from [Google Takeout](https://takeout.google.com)

### Quick Start

1. **Download Your Data**
   ```
   Visit: https://takeout.google.com
   Select: Hangouts/Chat → Export → Download
   Extract: The downloaded ZIP file
   ```

2. **Open the Viewer**
   - Download `google_chat_takeout_reader.html`
   - Double-click to open in your browser
   

3. **Load Your Chat History**
   - Click "Choose Directory" 
   - Select your extracted Takeout folder
   - Browse your chat history!

## 🎯 How to Use

### 📂 **Loading Your Data**
The app automatically scans your Takeout directory structure and identifies:
- **Chat Messages**: `messages.json` files
- **Chat Metadata**: `group_info.json` files  
- **Media Files**: Images, audio, and attachments
- **Chat Participants**: Member information and roles

### 🔍 **Searching & Navigation**
- **Find Chats**: Use the sidebar search to find chats by name or participants
- **Search Messages**: Use the header search to find specific messages
- **Browse History**: Scroll through messages or use pagination controls
- **Jump to Message**: Click the message counter to jump to a specific message

### 🎨 **Customization**
- **Filter Views**: Show only messages with images
- **Hide Members**: Exclude specific participants from view
- **Responsive Design**: Automatically adapts to your screen size

## 🏗️ Architecture

### **Single-File Design**
This is a completely **self-contained web application**:
- ✅ No server installation required
- ✅ No external dependencies to install
- ✅ Works entirely in your browser
- ✅ Your data never leaves your device

### **Browser APIs Used**
- **File System Access API**: For reading Takeout directories
- **Blob URLs**: For displaying images and media
- **Local Storage**: For caching and performance

### **Privacy First**
- 🔒 **100% Client-Side**: Your chat data never leaves your computer
- 🔒 **No Network Requests**: Works completely offline
- 🔒 **No Data Collection**: Zero tracking or analytics

## 🛠️ Technical Details

### **Supported Data**
- **Message Types**: Text, images, audio, files, reactions
- **Chat Types**: Direct messages, group chats, Spaces
- **Metadata**: Timestamps, participants, chat names, emoji avatars
- **Attachments**: All file types supported by Google Chat

### **Performance**
- **Smart Caching**: Messages cached in memory for fast navigation
- **Lazy Loading**: Images loaded on demand
- **Efficient Rendering**: Handles large chat histories smoothly

### **Browser Compatibility**
| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 86+ | ✅ Full Support |
| Edge | 86+ | ✅ Full Support |
| Safari | 14+ | ✅ Full Support |
| Firefox | - | ❌ File System API not supported |

## 📝 Development

### **Project Structure**
```
google-chat-takeout-viewer/
├── google_chat_takeout_reader.html    # Main application file
├── README.md                          # This file
├── .gitignore                         # Git ignore rules
└── .github/
    └── copilot-instructions.md        # AI development guidelines
```

### **Contributing**
1. Fork the repository
2. Make your changes to `google_chat_takeout_reader.html`
3. Test with various Takeout exports
4. Submit a pull request

## 📄 License

This project is open source. Feel free to use, modify, and distribute.

## 🆘 Troubleshooting

### Common Issues

**"Browser not supported"**
- Use Chrome 86+, Edge 86+, or Safari 14+
- Firefox doesn't support File System Access API yet

**"No chats found"**
- Ensure you selected the correct Takeout directory
- Look for a folder containing "Hangouts" or "Chat" data

**"Images not loading"**
- Images must be in the same Takeout directory structure
- Check browser console for file access errors

**"Search not working"**
- Clear your browser cache and reload
- Ensure JavaScript is enabled

## 🤝 Support

- **Issues**: Report bugs on GitHub Issues
- **Feature Requests**: Open a GitHub Discussion
- **Questions**: Check existing issues or start a discussion

---

**Made with ❤️ for the Google Chat community**