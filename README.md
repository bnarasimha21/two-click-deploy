# Two-Click Deploy

Deploy web applications to the cloud with minimal effort. This tool uses speech-to-text transcription (Whisper) to capture your app requirements, generates a complete web page using GPT-4o-mini, and prepares it for deployment via the GitHub API.

## Features

- **Voice-Powered Input** -- Describe your desired web app using your microphone via OpenAI Whisper
- **AI Code Generation** -- Automatically generates a complete `index.html` using GPT-4o-mini
- **GitHub Integration** -- Interact with GitHub repos programmatically via PyGithub
- **Gradio Web Interface** -- Simple browser-based UI for transcription and deployment

## Tech Stack

- **Language:** Python
- **Speech Recognition:** OpenAI Whisper (via Hugging Face Transformers)
- **LLM:** OpenAI GPT-4o-mini
- **GitHub API:** PyGithub
- **Web Interface:** Gradio
- **Audio Processing:** torchaudio

## Setup / Installation

```bash
git clone https://github.com/bnarasimha21/two-click-deploy.git
cd two-click-deploy
pip install -r requirements.txt
```

### Environment Variables

```bash
export OPENAI_API_KEY="your-openai-api-key"
```

## Usage

### Run the App

```bash
python app.py
```

1. Open the Gradio interface in your browser
2. Click the microphone to describe the web application you want (e.g., "Generate a simple fashion website")
3. The app transcribes your speech and uses GPT-4o-mini to generate a complete HTML page

### Generate HTML via CLI

```bash
python llm.py
```

Directly generates an `index.html` from a text prompt using GPT-4o-mini.

## License

MIT
