###🌿 Aura: Your Wellness Companion

Aura is a compassionate, single-page conversational AI designed to support your daily mental and emotional well-being. Built using a combination of modern HTML, Tailwind CSS for aesthetics, and the Gemini API for intelligent, empathetic responses, Aura provides instant validation, affirmation, and gentle wellness tips.

###✨ Features

Empathetic AI Persona: Aura is configured with a warm, supportive, and non-judgmental system instruction to prioritize your emotional state.

Onboarding Flow: Personalizes the experience by asking for your name and occupation (student/employee) to tailor its advice.

Session Persistence: Uses the browser's sessionStorage to remember your chat history and profile (name/occupation) between sessions.

Responsive & Aesthetic Design: Features a calm, green, wellness-focused design using Tailwind CSS, ensuring a great experience on both mobile and desktop.

Real-time Interaction: Includes a typing indicator and client-side handling for immediate feedback during AI processing.

###🛠️ Setup and Prerequisites

Since Aura is a single HTML file, setup is minimal, but it requires access to the Google Gemini API.

####API Key Configuration

The current code is designed to function within a specific cloud environment where the API key is automatically injected. However, if you run this file locally, you must replace the placeholder.

Get Your Key: Obtain a Google Gemini API key.

Update the Code: Open the aura_wellness_chatbot.html file and locate the following line near the top of the main <script> block:

#####const API_KEY = "AIzaSyD-YOUR-REAL-SECRET-KEY-HERE"; 


Replace "AIzaSyD-YOUR-REAL-SECRET-KEY-HERE" with your actual API key (Note: Exposing API keys in client-side code is generally discouraged for production apps and is done here for simplicity).

Running Locally

Save the code as a single file (e.g., aura_wellness_chatbot.html).

Open the file directly in your web browser.

###🚀 Usage

Start: Upon launch, Aura will begin the onboarding process by asking for your name.

Profile Setup: Enter your name, followed by your occupation (student or employee) as prompted.

Conversation: Once onboarding is complete, Aura will give a welcoming message. You can now chat about your feelings, stress, anxiety, or general well-being.

Interaction: Use the input box to type your message and press Enter or click the Send button (paper airplane icon).

###💻 Technical Stack

HTML5: Core structure.

CSS: Inlined custom styles and Tailwind CSS utility classes (via CDN).

JavaScript (ES6): Core application logic, including chat state management, API calls, and UI rendering.

Gemini API (gemini-2.5-flash-preview-09-2025): Used for generating the AI's conversational and therapeutic responses.

Lucide Icons (via CDN): Used for the leaf and send icons.

sessionStorage: Used for lightweight, client-side persistence of user profile and chat history.

###⚠️ Notes on API Key Security

This application uses a client-side API call for simplicity. For any production application, the secure solution is to proxy the API request through a private backend server (e.g., Node.js, Python), which reads the API key from a secure .env file and hides it from the public browser client.