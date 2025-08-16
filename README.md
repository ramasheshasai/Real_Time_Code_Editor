# Real-time Collaborative Code Editor

A real-time collaborative code editor built with React and Socket.IO that allows multiple users to code together simultaneously. Perfect for pair programming, code reviews, and collaborative development sessions.

## ✨ Features

- **Real-time Collaboration**: Multiple users can edit code simultaneously with instant synchronization
- **Live User Presence**: See who's currently in the room with avatar indicators
- **Room-based Sessions**: Create or join coding rooms using unique room IDs
- **Syntax Highlighting**: JavaScript syntax highlighting with CodeMirror
- **Auto-completion**: Automatic bracket and tag closing
- **Responsive Design**: Works seamlessly across different screen sizes
- **Toast Notifications**: Real-time notifications for user join/leave events
- **Copy Room ID**: Easy sharing of room IDs with clipboard integration

## 🚀 Demo

![Real-time Code Editor Demo](https://via.placeholder.com/800x400/282a36/4aed88?text=Real-time+Code+Editor)

## 🛠️ Tech Stack

**Frontend:**
- React 17
- Socket.IO Client
- CodeMirror (Code Editor)
- React Router DOM
- React Hot Toast (Notifications)
- React Avatar

**Backend:**
- Node.js
- Express.js
- Socket.IO Server

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/realtime-code-editor.git
   cd realtime-code-editor
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables** (optional)
   Create a `.env` file in the root directory:
   ```env
   REACT_APP_BACKEND_URL=http://localhost:5000
   PORT=5000
   ```

## 🚀 Usage

### Development Mode

1. **Start the development server**
   ```bash
   npm run server:dev
   ```

2. **In another terminal, start the React app**
   ```bash
   npm run start:front
   ```

3. **Open your browser**
   Navigate to `http://localhost:3000`

### Production Mode

1. **Build and start the application**
   ```bash
   npm start
   ```

2. **Open your browser**
   Navigate to `http://localhost:5000`

## 📖 How to Use

1. **Create a Room**: Click "new room" to generate a unique room ID
2. **Join a Room**: Enter an existing room ID and your username
3. **Start Coding**: Begin typing and see real-time collaboration in action
4. **Share Room**: Use the "Copy ROOM ID" button to invite others
5. **Leave Room**: Click "Leave" to exit the collaborative session

## 🏗️ Project Structure

```
realtime-code-editor/
├── public/
│   ├── index.html
│   ├── code-sync.png
│   └── ...
├── src/
│   ├── components/
│   │   ├── Client.js          # User avatar component
│   │   └── Editor.js          # CodeMirror editor wrapper
│   ├── pages/
│   │   ├── Home.js            # Landing page
│   │   └── EditorPage.js      # Main editor interface
│   ├── Actions.js             # Socket.IO action constants
│   ├── socket.js              # Socket.IO client configuration
│   ├── App.js                 # Main app component
│   └── ...
├── server.js                  # Express + Socket.IO server
└── package.json
```

## 🔧 Available Scripts

- `npm run start:front` - Start React development server
- `npm run server:dev` - Start backend server with nodemon
- `npm run server:prod` - Start backend server in production
- `npm start` - Build and start production server
- `npm run build` - Build React app for production
- `npm test` - Run tests

## 🌐 Socket.IO Events

| Event | Description |
|-------|-------------|
| `JOIN` | User joins a room |
| `JOINED` | Broadcast when user successfully joins |
| `CODE_CHANGE` | Real-time code synchronization |
| `SYNC_CODE` | Sync code with newly joined users |
| `DISCONNECTED` | User leaves the room |

## 🎨 Customization

### Themes
The editor uses the Dracula theme by default. You can change it in `src/components/Editor.js`:

```javascript
theme: 'dracula', // Change to your preferred theme
```

### Language Support
Currently supports JavaScript. Add more languages by importing CodeMirror modes:

```javascript
import 'codemirror/mode/python/python';
import 'codemirror/mode/css/css';
```

## 🚀 Deployment

### Heroku
1. Create a Heroku app
2. Set environment variables
3. Deploy using Git or GitHub integration

### Vercel/Netlify
1. Build the React app: `npm run build`
2. Deploy the `build` folder
3. Configure server endpoints

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -am 'Add feature'`
4. Push to branch: `git push origin feature-name`
5. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [CodeMirror](https://codemirror.net/) for the excellent code editor
- [Socket.IO](https://socket.io/) for real-time communication
- [React](https://reactjs.org/) for the UI framework

## 📞 Support

If you have any questions or run into issues, please open an issue on GitHub or contact ramasheshasai_s@srmap.edu.in

---

⭐ **Star this repository if you found it helpful!**
