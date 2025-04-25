# AI Flashcard Generator App

This is a full-stack web app that generates flashcards from online resources using DeepSeek AI and Google Custom Search.

## Features
- Enter any topic and automatically search for relevant articles/blogs.
- Extract content from selected resources.
- Generate flashcards (Q&A) using DeepSeek AI.
- Review flashcards with a modern React interface.

---

## Installation & Setup

### 1. Clone the repository
```
git clone <your-repo-url>
cd windsurf-playground-1
```

### 2. Install dependencies (for all parts)
```
npm install            # Installs root dev dependencies and sets up scripts
cd backend && npm install   # Installs backend dependencies
cd ../frontend && npm install   # Installs frontend dependencies
cd ..   # Return to project root
```

### 3. Set up API Keys (.env)
Create a `.env` file inside the `backend` directory with the following:
```
GOOGLE_API_KEY=your_google_api_key_here
GOOGLE_CSE_ID=your_google_custom_search_engine_id_here
DEEPSEEK_API_KEY=your_deepseek_api_key_here
```
- [Get a Google API Key & Custom Search Engine ID](https://developers.google.com/custom-search/v1/overview)
- [Get a DeepSeek API Key](https://platform.deepseek.com/)

### 4. Run the App (Both Servers Together)
From the project root:
```
npm run dev
```
- This will start both the backend (on port 5000) and frontend (on port 3000) in development mode.
- Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## Usage
1. Enter a topic (e.g., "Photosynthesis") and click **Search Resources**.
2. Select a resource and click **Extract** to fetch its content.
3. Click **Generate Flashcards** to create Q&A pairs using DeepSeek AI.
4. Review flashcards interactively (flip, next, previous).

---

## Project Structure
```
backend/    # Node.js Express API (resource search, content extraction, AI flashcard generation)
frontend/   # React app (UI for search, extraction, flashcard review)
```

---

## Notes
- Make sure your API keys are kept private and **never commit your .env file**.
- For production deployment, further configuration is recommended.

---

Enjoy learning with AI-powered flashcards!