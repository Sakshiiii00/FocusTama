# FocusTama 🐾 - Your Retro Productivity Pet

**FocusTama is an AI-powered web application that transforms productivity into an engaging experience through a virtual pixel-art companion. Inspired by the iconic Tamagotchi, the application encourages users to stay focused, complete tasks, and maintain healthy work habits by rewarding consistent productivity with their pet's growth and well-being.

This project was built for the **"Blast from the Past: With a Modern Twist"** theme, reviving the beloved virtual pet concept with modern web technologies, including a dynamic UI, browser notifications, and a conversational AI companion powered by Google's Gemini.

**[[▶️ Live Demo Link Here]](https://focustama.vercel.app/)**

<img width="1908" height="976" alt="Image" src="https://github.com/user-attachments/assets/9001aba8-3a62-4e7c-88fb-244f5c05d634" />

### Focus Streak Graph
A GitHub-style contribution graph visualizes your productivity over the last 70 days.

![Graph View](https://github.com/user-attachments/assets/111a8d2b-0652-4045-946d-8c29f82406e5)

### Conversational AI Companion
Chat with your pet! It uses the Google Gemini API to provide unique, encouraging, and context-aware responses.

![AI Chat Example](https://github.com/user-attachments/assets/44f1a93e-c1bc-403b-8f29-56313dc556fe)

---

## ✨ Core Features

* **Interactive Virtual Pet:** Nurture a charming pixel-art companion whose happiness, hunger, and energy levels dynamically change based on your productivity and interactions.

* **Integrated Task Management:** Stay organized with a built-in task manager. Each Pomodoro session begins only after selecting a task, ensuring every focus session is linked to a meaningful goal.

* **Gamified Productivity System:**
    * **Focus Rewards:** Completing focus sessions boosts your pet's happiness and encourages consistent productivity.
    * **Healthy Breaks:** During break sessions, interact with and feed your pet to restore its energy and promote balanced work habits.
    * **Dynamic Consequences:** Neglecting your pet over time decreases its health and mood, motivating regular engagement and self-care.

* **Pet Evolution:** Unlock an upgraded version of your virtual companion after successfully completing five focus sessions, providing long-term motivation and a rewarding sense of progression.

* **AI-Powered Companion:** Chat with your virtual pet through Google Gemini AI, which delivers personalized, supportive, and context-aware conversations for a more engaging experience.

* **Dynamic Day & Night Cycle:** The application's interface automatically adapts to your local time with smooth transitions between day, evening, and night. Your pet sleeps at night, temporarily pausing stat decay for added realism.

* **Productivity Streak Tracker:** Monitor your consistency using a GitHub-inspired contribution graph that visualizes your focus sessions over the past 70 days.

* **Persistent Progress:** Your pet's status, completed tasks, achievements, and application data are automatically stored in the browser's `localStorage`, allowing you to continue exactly where you left off.

* **Retro Gaming Experience:** Enjoy nostalgic pixel-art visuals, CRT-inspired effects, and immersive 8-bit sound effects that combine classic gaming aesthetics with modern web technologies.

---

## 🛠️ Technology Stack

This project was built from the ground up with a focus on clean, framework-free code.

*   **Frontend:** Pure HTML5, CSS3, and JavaScript (ES6+).
*   **Graphics:** HTML `<canvas>` for smooth, sprite-based animations.
*   **Styling:** CSS variables for easy theming (like the day/night cycle) and Flexbox/Grid for responsive layouts.
*   **AI:** [Google AI Studio (Gemini API)](https://aistudio.google.com/) for natural language conversation.
*   **Storage:** Browser `localStorage` for all state persistence.
*   **Notifications:** Web Notifications API for reminders.
*   **Audio:** HTML5 `<audio>` for sound effects.

---

## 📂 File Structure

The project is organized into a clean and intuitive structure:

```
focustama/
│
├── 📄 index.html # The main HTML file containing the app structure.
├── 📄 style.css # All styles for the UI, device, and animations.
├── 📄 script.js # The core application logic, state, and game loops.
├── 📄 config.js # Holds the secret API key (ignored by Git).
├── 📄 README.md # You are here!
├── 📄 .gitignore # Tells Git to ignore sensitive files like config.js.
│
└── 📁 assets/
├── 📁 audio/
│ ├── 🔊 click.mp3
│ ├── 🔊 success.mp3
│ ├── 🔊 feed.mp3
│ ├── 🔊 sad.mp3
│ └── 🔊 evolve.mp3
│
└── 📁 images/
├── 🖼️ icon.png
├── 🖼️ puppy-idle.png
├── 🖼️ puppy-happy.png
├── 🖼️ puppy-sad.png
├── 🖼️ puppy-evo-idle.png
├── 🖼️ puppy-evo-happy.png
└── 🖼️ puppy-evo-sad.png
```
---

## 🚀 Getting Started

To run FocusTama on your local machine, follow these simple steps.

### Prerequisites

*   A modern web browser (Chrome, Firefox, Edge).
*   A code editor (like VS Code).
*   The **Live Server** extension for VS Code is highly recommended to avoid potential CORS issues with the AI API.

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/focustama.git
    cd focustama
    ```

2.  **Create your configuration file:**
    *   In the root of the project, create a new file named `config.js`.
    *   This file will hold your secret API key and is ignored by Git (see `.gitignore`).

3.  **Get your Google AI API Key:**
    *   Visit [aistudio.google.com](https://aistudio.google.com/).
    *   Log in and click **"Get API key"** -> **"+ Create API key in new project"**.
    *   Copy the generated key.

4.  **Add your API Key to `config.js`:**
    *   Open `config.js` and add the following line, pasting your key inside the quotes:
    ```javascript
    const GOOGLE_API_KEY = 'PASTE_YOUR_GOOGLE_AI_API_KEY_HERE';
    ```

5.  **Run the application:**
    *   If you have the **Live Server** extension in VS Code, simply right-click `index.html` and choose "Open with Live Server".
    *   Otherwise, you can open `index.html` directly in your browser.

Your FocusTama should now be running locally!

---

## 💡 Future Development

While this version is feature-complete, here are some exciting ideas for future expansion:
*   **Focus Shop:** Earn a currency from completed tasks to buy accessories (hats, scarves) or new backgrounds for your pet.
*   **More Mini-Games:** Add more ways to "Play" with your pet to increase happiness.
*   **Weekly Goals & Achievements:** Implement a system for weekly challenges (e.g., "Complete 10 focus sessions") to encourage long-term consistency.
*   **Browser Extension:** A companion extension to show your pet's status at a glance and gently remind you to stay off distracting sites during a focus session.

---

Thank you for checking out FocusTama! I hope it helps you stay focused and brings a smile to your face.
