🤖 Jarvis – AI Powered Voice Assistant (Python)

An AI-powered voice assistant built with Python that listens for voice commands, performs web-based actions, fetches news, plays music, and generates intelligent responses using OpenAI.

Inspired by Alexa and Google Assistant.

✨ Features

🎤 Wake-word detection ("Jarvis")

🗣 Speech-to-text using SpeechRecognition

🔊 Text-to-speech using pyttsx3

🌐 Open popular websites (YouTube, Google, Facebook, College site)

🎵 Play songs from a custom music library

📰 Fetch latest Indian headlines via NewsAPI

🤖 AI-powered responses using OpenAI API

🎧 MP3 playback using pygame (gTTS fallback supported)

🏗️ Tech Stack

Python 3.9+

SpeechRecognition

PyAudio

pyttsx3

gTTS

pygame

requests

OpenAI Python SDK

📂 Project Structure
jarvis-voice-assistant/
│                
├── main.py                
├── musicLibrary.py        
├── requirements.txt        
└── README.md        
⚙️ Installation
1️⃣ Clone the Repository    
git clone https://github.com/yourusername/jarvis-voice-assistant.git
cd jarvis-voice-assistant    
2️⃣ Create Virtual Environment (Recommended)
python -m venv venv
venv\Scripts\activate     # Windows
source venv/bin/activate  # Mac/Linux    
3️⃣ Install Dependencies
pip install -r requirements.txt    

Or manually:

pip install speechrecognition pyttsx3 gtts pygame requests openai pyaudio
🔑 Environment Variables
    
Set your API keys securely.    

Windows (PowerShell)
setx OPENAI_API_KEY "your_openai_key"
setx NEWS_API_KEY "your_newsapi_key"
Mac/Linux
export OPENAI_API_KEY="your_openai_key"
export NEWS_API_KEY="your_newsapi_key"

Restart terminal after setting environment variables.

▶️ Running the Assistant
python main.py

You should hear:

Initializing Jarvis...

Say:

Jarvis

Then give your command.

🧠 Example Commands
Command	Action
Open YouTube	Opens YouTube
Open Google	Opens Google
Play believer	Plays song from music library
Give me news	Reads latest headlines
What is AI?	AI-generated short explanation
🎵 Example musicLibrary.py
music = {
    "believer": "https://youtu.be/7wtfhZwyrcc",
    "faded": "https://youtu.be/60ItHLz5WEA"
}
🔐 Security Best Practices

Never hardcode API keys.

Always use .env or system environment variables.

Add .env to .gitignore.

Example .gitignore:

venv/
__pycache__/
.env
temp.mp3
⚠️ Known Limitations

Requires internet for:

Google speech recognition

News API

OpenAI responses

Wake-word detection is basic (not ML-based)

Short microphone timeout (can be adjusted)

🚀 Future Improvements

GUI using Tkinter or PyQt

Spotify API integration

System control commands

Better wake-word detection

Offline speech recognition mode

Docker deployment

🧪 Requirements.txt (Recommended)
speechrecognition
pyttsx3
gtts
pygame
requests
openai
pyaudio
📜 License

MIT License

🙌 Contributing

Pull requests are welcome. For major changes, open an issue first to discuss improvements.

⭐ Show Your Support

If you like this project, give it a ⭐ on GitHub!

If you want, I can now provide:

🔥 A cleaned and optimized production version of your code

🧠 Upgrade to latest OpenAI API format

🐳 Dockerized version

🖥️ Add a simple GUI

📦 Convert into an installable Python package
