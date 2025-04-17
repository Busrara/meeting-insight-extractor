# meeting-insight-extractor

Meeting Insight Extractor is an AI-powered assistant designed to transform meeting transcripts, Zoom/Teams calls, or chat conversations into structured action items, summaries, sentiment analysis, and even role-based highlights. By leveraging advanced language models and natural language processing (NLP) techniques, Meeting Insight Extractor helps teams capture key decisions and tasks efficiently without manually sifting through long transcripts.

🚀 Features

Speech-to-Text: Transcribe audio files (e.g., Zoom, Teams) into text using Whisper API.
Automatic Summarization: Generate concise summaries and key insights from meeting transcripts.
Action Item Extraction: Identify and extract actionable tasks such as "John will prepare the report by Friday."
Sentiment & Tone Analysis: Understand the mood and sentiment of the conversation—who was positive, who was neutral, and who might need follow-up.
Multi-Language Support: Supports multiple languages, including English and Turkish.
Speaker-Based View: View contributions by different speakers in the meeting.
⚙️ Technology Stack

OpenAI API: For summarization and action item extraction using GPT-3.5 Turbo.
Whisper: For speech-to-text transcription from audio files.
Python: The project is developed in Python using libraries such as openai, whisper, regex, and dotenv.
Pandas & Matplotlib: For data handling and visualization (if needed).
🔧 Installation

Clone the repository:
git clone https://github.com/your-username/meeting-insight-extractor.git
Navigate to the project directory:
cd meeting-insight-extractor
Install the required dependencies:
pip install -r requirements.txt
Create a .env file to store your API keys:
OPENAI_API_KEY=your_openai_api_key_here
🛠️ Usage

1. Transcribing Audio:
To transcribe audio files into text, call the transcribe_audio() function:

from utils import transcribe_audio

text = transcribe_audio("path_to_audio_file.wav")
print(text)
2. Generate Summary:
You can generate a summary of a transcript by using:

from utils import generate_summary

with open("transcript.txt", "r") as f:
    transcript = f.read()

summary = generate_summary(transcript)
print("Summary:", summary)
3. Extract Action Items:
To extract action items from the transcript:

from utils import extract_action_items

with open("transcript.txt", "r") as f:
    transcript = f.read()

actions = extract_action_items(transcript)
for action in actions:
    print(action)
📈 Future Features

Integration with calendar apps to directly create tasks and reminders.
Support for more advanced sentiment analysis.
Real-time transcription and summary for live meetings.
Enhanced speaker identification and role-based task assignment.
🔗 Contributing

If you'd like to contribute to Meeting Insight Extractor, feel free to fork the repository and submit a pull request. Contributions are welcome!

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

Enjoy using Meeting Insight Extractor to enhance your meeting productivity! 🚀

