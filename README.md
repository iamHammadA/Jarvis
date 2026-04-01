# Jarvis – AI Voice Assistant 🤖

**Jarvis** is a personal AI assistant built in Python that listens to your voice, responds intelligently, performs web searches, plays media, and interacts using Google’s Generative AI. This project combines **speech recognition, text-to-speech, web automation, YouTube & image search, and AI-based chat** into a single, powerful assistant.

---

## 🚀 Features

- **Voice Activation:** Say `"Jarvis"` to activate the assistant.  
- **Voice Recognition:** Uses `speech_recognition` to understand natural language commands.  
- **Text-to-Speech:** Responds using `pyttsx3` for a natural voice assistant experience.  
- **Web Automation:** Automatically opens websites like Google, YouTube, Pinterest, Facebook, Amazon, and more.  
- **YouTube & Media Control:** Search and play YouTube videos or music directly by voice.  
- **Image Search:** Search for images on Google using voice commands.  
- **AI Chat Assistant:** Uses Google Generative AI (`gemini-1.5-flash`) to answer questions intelligently.  
- **Extensible Commands:** Easily add new voice commands and actions.  

---

## 📂 Project Structure


Jarvis/
│
├── jarvis.py # Main script
├── names_of_audio.py # Stores URLs for media commands
├── youtube_api # File containing YouTube API key
├── api_key # File containing Google API key
├── search_engine_id # File containing Google Custom Search Engine ID
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## 🛠️ Installation

1. **Clone the repository:**

```bash
git clone https://github.com/iamHammadA/Jarvis.git
cd Jarvis
Install dependencies:
pip install -r requirements.txt
Configure API keys:
youtube_api → Your YouTube Data API key
api_key → Your Google Custom Search API key
search_engine_id → Your Google Custom Search Engine ID

Make sure your microphone is connected and working.

💻 Usage
Run the assistant:
python jarvis.py
Activate Jarvis: Say "Jarvis" to start giving commands.
Examples of commands:
Open websites: "open Google", "open YouTube", "open Facebook"
Play media: "play Yah Dunya", "play Jhol"
Search images: "search for a sunset"
AI chat: Ask any question after activation, and Jarvis will answer using Google Generative AI.
🔧 How It Works
Speech Recognition:
Listens continuously via the microphone.
Detects the keyword "Jarvis" to activate commands.
Command Parsing:
Uses Python string matching and numpy.char.lower to detect commands.
Web & Media Actions:
Opens URLs in your browser using webbrowser
Plays YouTube videos or searches images using YouTube API & Google Custom Search API.
AI Responses:
Integrates with google.generativeai for natural language responses.
Outputs results via text-to-speech using pyttsx3.
⚡ Dependencies

Include these in requirements.txt:

pyttsx3
speechrecognition
requests
beautifulsoup4
pytube
mediapipe
opencv-python
google-generativeai
numpy
🎨 Customization
Add more websites or commands in jarvis.py under the command logic.
Update names_of_audio.py for more pre-defined media URLs.
Adjust the speech recognition sensitivity by modifying recognizer.adjust_for_ambient_noise(source).
🖼️ Screenshots / Demo

(Optional: Add screenshots or GIFs of Jarvis in action to showcase your project)

⚖️ License

This project is open-source. You are free to modify, reuse, or improve it for personal or educational projects.

📫 Contact
GitHub: iamHammadA
Instagram: @iamHammadA

---

✅ **Next Steps Recommendation:**  

1. Save this as `README.md` in your project folder.  
2. Commit & push it to GitHub:

```bash
git add README.md
git commit -m "Add detailed professional README"
git push
