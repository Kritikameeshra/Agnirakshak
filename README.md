# AgniRakshak 🔥

**AgniRakshak** is an AI-powered chatbot assistant focused on fire safety regulations and compliance. It leverages Google Generative AI and Pinecone vector search to provide accurate, context-aware answers to fire safety-related queries.

![AGNIRAKSHAK](AGNIRAKSHAK.gif)

## Features

- **Conversational Fire Safety Assistant**: Ask questions about fire safety, standards, and regulations.
- **AI-Powered Retrieval**: Uses Google Generative AI and Pinecone for context-aware answers.
- **Keyword Filtering**: Only responds to fire safety-related queries; blocks harmful or unrelated content.
- **Modern React UI**: Clean, responsive interface with chat, input, and helpful UI components.

## Getting Started

### Prerequisites

- Node.js (v16+ recommended)
- npm

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd fire
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root directory with the following keys:
   ```
   REACT_APP_PINECONE_API_KEY=your-pinecone-api-key
   REACT_APP_PINECONE_INDEX=your-pinecone-index
   REACT_APP_GOOGLE_API_KEY=your-google-api-key
   ```

### Running the App

```bash
npm start
```

The app will run locally at [http://localhost:3000](http://localhost:3000).

## Project Structure

```
fire/
├── public/
│   ├── index.html
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── Navbar.jsx, Footer.jsx, Loader.jsx, Input.jsx, Messages.jsx, UserMessage.jsx, BotMessage.jsx, Dictaphone.jsx
│   ├── ChatbotAPI.js
│   ├── index.js
│   ├── lang.mjs
│   ├── styles.css
│   └── index.css
├── package.json
└── AGNIRAKSHAK.gif
```

## How it Works

- The main chatbot logic is in `src/index.js`.
- User messages are processed and sent to the AI backend via `ChatbotAPI.js`.
- `lang.mjs` handles the AI logic, using Pinecone for vector search and Google Generative AI for generating responses.
- Only fire safety-related queries are answered; others are politely declined.
- Harmful or dangerous queries are blocked.

## Customization

- **UI**: Modify or extend components in `src/components/`.
- **AI Logic**: Adjust keyword lists or prompt templates in `src/lang.mjs`.

## Dependencies

- React
- @google/generative-ai
- @langchain/google-genai
- @langchain/pinecone
- @pinecone-database/pinecone
- styled-components
- react-icons
- react-router-dom

---

**Author:** Kritika 