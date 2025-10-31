Gemini Chat Companion: The Adaptive Vibe Chat 💬

The Gemini Chat Companion is a lightweight, responsive chat application designed to demonstrate dynamic, contextual AI interaction. Unlike standard chatbots, this companion uses its system instructions to analyze the user's current mood or "vibe" (e.g., stressed, excited, curious) and adjusts its tone and response style to provide a highly personalized and empathetic conversation.

The entire application is built into a single HTML file for maximum simplicity and portability, running entirely client-side using CDNs.

✨ Features

Adaptive Persona: The AI analyzes the user's messages to infer mood and customizes its conversational tone to be supportive, empathetic, or enthusiastic, depending on the user's state.

Single-File Deployment: The entire application (HTML, CSS, React, and logic) is contained in one index.html file.

Fully Responsive Design: The interface adapts seamlessly, appearing as a full-screen mobile app on phones and a clean, centered chat card on desktop browsers.

Client-Side State: Chat history is managed entirely in the browser's memory, requiring no database setup (history resets on refresh).

🛠️ Technologies Used

Category

Tool / Technology

Purpose

Core AI

Gemini API (gemini-2.5-flash)

Powers the adaptive conversational intelligence.

Frontend

React (via CDN)

Provides the component structure and state management.

Styling

Tailwind CSS (via CDN)

Used for all responsive and modern UI styling.

Build

Babel (via CDN)

Compiles the React JSX directly in the browser.

Deployment

GitHub Pages

Recommended platform for free, instant static hosting.

🚀 Setup and Installation

A. Local Run (Zero Configuration)

To run this application, you only need a modern web browser.

Obtain the Code: Save the index.html file provided in the editor to your local computer.

Acquire API Key: You must get a personal Gemini API Key from Google AI Studio.

Insert Key: Open the index.html file in a text editor (like VS Code or Notepad). Locate the apiKey variable near the top of the <script type="text/babel"> block and replace the empty quotes with your actual key:

const apiKey = "YOUR_GEMINI_API_KEY_HERE"; // <-- Update this line


Run: Double-click the saved index.html file. It will open directly in your web browser.

B. Deployment via GitHub Pages (Recommended)

This allows you to host the app online for free using a public URL.

Commit Code: Commit the API-key-updated index.html file to the root of a public GitHub repository (e.g., gemini-chat-app).

Enable Pages:

In your repository, go to Settings > Pages.

Set "Build and deployment" to Deploy from a branch.

Set the Branch to main (or master) and the folder to / (root).

Save: Click Save. GitHub will deploy your site in about one minute.

Access: Access your live app at the resulting GitHub Pages URL (e.g., https://[your-username].github.io/gemini-chat-app/).

🧠 How AI Helped in Development

This project serves as a direct demonstration of Prompt Engineering and the contextual power of the Gemini API.

The core functionality of the "Adaptive Companion" relies on a detailed System Instruction provided to the model with every request. This instruction explicitly mandates the following complex behavior:

Analyze the User Vibe: The model is told to first determine the user's emotional state.

Dynamically Adjust Tone: Based on the analysis, the model must change its conversational approach (e.g., be soothing for "stressed" users, or celebratory for "excited" users).

This process showcases how the AI can manage both the task (answering the question) and the emotional context (managing the tone) simultaneously, creating a significantly more engaging and human-like interaction than a standard API call.
