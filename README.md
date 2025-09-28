# Real-Time Legal Transcription App

A modern web application for real-time legal transcription with AI-powered response suggestions. Perfect for call centers, legal helplines, and customer service scenarios.

## Features

### 🎙️ Real-Time Transcription
- Live conversation simulation with realistic typing effects
- User messages on the left, operator responses on the right
- Typing indicators for natural conversation flow
- Auto-scrolling transcript window

### 🤖 Smart AI Suggestions
- **Only appears when questions are asked**
- Context-aware legal response suggestions
- 2 AI options with confidence scoring
- One-click response selection and integration

### ⚖️ Legal Example Scenario
- Eviction notice consultation
- User asks: "What should I do?", "Is this legal?", "What documents do I need?"
- AI provides specific, actionable responses for each question type

### 🎨 Modern UI/UX
- Clean, professional interface
- Responsive design for all devices
- Smooth animations and transitions
- Glassmorphism design with backdrop blur effects

## Getting Started

### Option 1: Direct Browser Opening
1. **Open the file directly**
   ```bash
   # Simply double-click or open in any modern web browser
   open realtime-transcription.html
   ```

### Option 2: Local Server (Recommended)
1. **Start a local server**
   ```bash
   # Python 3
   python3 -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   
   # Node.js (if you have it)
   npx http-server
   ```

2. **Open in browser**
   ```
   http://localhost:8000/realtime-transcription.html
   ```

## How to Use

1. **Click the Play button** to start the demo conversation
2. **Watch the conversation unfold** with realistic typing delays
3. **When the user asks a question**, AI suggestions appear on the right
4. **Operator can select a suggestion** to continue the conversation
5. **Use controls** to pause, resume, or reset the demo

## Controls

- **▶️ Play**: Start the demo conversation
- **⏸️ Pause**: Pause the simulation
- **🔄 Reset**: Clear and restart the demo

## Browser Compatibility

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## File Structure

```
legal_rtt/
├── realtime-transcription.html    # Main application (all-in-one)
├── requirements.txt               # Setup instructions
└── README.md                     # This documentation
```

## Customization

### Adding New Scenarios
Edit the `conversation` array in the JavaScript section to add new conversation flows:

```javascript
this.conversation = [
    {
        speaker: 'user',
        text: 'Your question here',
        isQuestion: true,
        delay: 2000
    },
    // ... more messages
];
```

### Customizing AI Responses
Modify the `aiResponses` object to add new response types:

```javascript
this.aiResponses = {
    'your_keyword': [
        {
            type: 'Response Type',
            text: 'Response text',
            confidence: 0.95
        }
    ]
};
```

## Technical Details

- **Pure HTML/CSS/JavaScript** - No external dependencies
- **Offline capable** - Works without internet after initial load
- **Responsive design** - Adapts to all screen sizes
- **Modern browser APIs** - Uses latest web standards

## Use Cases

- Legal call centers
- Customer service training
- Medical consultation demos
- Educational scenarios
- Any Q&A conversation simulation

## License

This project is for demonstration and educational purposes. Feel free to modify and use for your specific needs.
