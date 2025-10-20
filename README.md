🚀 CodeQuest: Learn Python by Playing 🐍

CodeQuest is an interactive, gamified web application designed to make learning Python fun and engaging. Conquer coding challenges, master lessons, and rise to the top of the leaderboard!

✨ Features

CodeQuest is packed with features to create a comprehensive and enjoyable learning experience:
🎮 Gamified Progression: Earn XP and coins for completing challenges, lessons, and puzzles. Keep your daily login streak alive to maximize rewards!
💻 Interactive Python Editor: Solve coding problems directly in the browser with a sleek editor that supports auto-indentation and line numbers.
🤖 AI-Powered Code Execution: Your code is executed securely via the Google Gemini API, providing instant output and error feedback against predefined test cases.
📚 Structured Lessons & Quizzes: Learn Python from the ground up with structured modules for Procedural Programming, OOP, and GUI development. Test your knowledge with a quiz at the end of each lesson.
🧩 Challenging Coding Puzzles: Put your problem-solving skills to the test with puzzles categorized by difficulty. Each comes with multiple test cases and helpful hints.
💡 AI Tutor Chatbot: Stuck on a concept? "CodeBot," our 24/7 AI tutor powered by Gemini, is always available to answer your Python questions.
🏆 Achievements & Certificates: Earn badges for mastering different areas of Python and receive printable certificates to showcase your accomplishments.
🌍 Global Leaderboard: See how you stack up against other learners worldwide, ranked by total XP.
🎥 Video Tutorials: Supplement your learning with a curated collection of YouTube tutorials for various Python topics.
🔐 User Authentication: A secure and persistent login/registration system using local storage to save your progress.
📱 Modern & Responsive UI: A sleek, dark-themed interface built with Tailwind CSS, featuring smooth animations and a design that looks great on any device.

🛠️ Tech Stack

This project is built with a modern, no-build-step toolchain:

Frontend: React, TypeScript, Tailwind CSS
AI & Backend Logic: Google Gemini API (@google/genai) for code execution and AI tutoring
State Management: React Context API & Hooks (useContext, useState, useEffect)
Persistence: Browser Local Storage (for user sessions, code progress, chat history)
Environment: Modern browser features like ES Modules and Import Maps (No build step required!)

🚀 Getting Started

Since this project is built without a traditional build step (like Webpack or Vite), you can run it easily with any local static server.

Clone the repository:
git clone https://github.com/your-username/codequest.git
cd codequest

Set up your API Key:
The application requires a Google Gemini API key. The app is designed to read this key from an environment variable (process.env.API_KEY) that the hosting environment provides. For simple local testing, you will need a server that can inject this variable.

Serve the files:
You can use any simple static server.

Using Node.js and serve:

# Install serve globally if you haven't already
npm install -g serve

# Run the server
serve -s .

📂 Project Structure
/
├── components/       # Reusable React components (Button, Header, Modals, etc.)
│   ├── icons/        # SVG icon components
│   └── ...
├── contexts/         # React context for global state (AuthContext)
├── data/             # Static data for challenges, lessons, quizzes, etc.
├── hooks/            # Custom hooks (useAuth for handling user logic)
├── pages/            # Top-level page components (LandingPage, DashboardPage)
├── services/         # Services that interact with external APIs (geminiService)
├── index.html        # The main HTML entry point with import maps
├── index.tsx         # The main React entry point
└── README.md         # This file!

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.
