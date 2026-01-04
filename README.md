## Bilingual AI Voice Assistant (Tamil & English)

Link: https://colab.research.google.com/drive/1IKPE7cnf6AdZ9zNESXGDCCpHaXdgYFv6?usp=sharing

A conversational AI voice assistant that understands and responds in both Tamil and English.
Built with Python and powered by Google’s Gemini LLM, this project runs entirely in Google Colab, making it accessible through a browser without any local setup.

The assistant supports voice-based interaction, real-time language switching, and end-to-end speech understanding and generation.

## Why This Matters in Industry

Multilingual and cross-lingual AI systems are critical for scaling AI to diverse and non-English-speaking user bases.

Demonstrates applied speech-to-text, LLM reasoning, and text-to-speech integration in a single pipeline.

Highlights work on low-resource language support, an important challenge in modern NLP.

Relevant to conversational AI, voice assistants, accessibility tools, and regional AI products.

Shows system-level AI design, not just isolated model usage.

## Features

Bilingual Conversation: Interact with the assistant in either Tamil or English.

AI-Powered Intelligence: Uses the Google Gemini 1.5 Flash model to understand context and generate relevant, human-like responses.

Dynamic Language Switching: Switch the active language at runtime using a button or voice command.

Voice-Based Interaction: Fully hands-free interaction using real-time speech recognition.

Zero Local Setup: Runs entirely in Google Colab with no local installation required.

## How It Works

The assistant follows a multi-step pipeline to process voice input and generate spoken responses.

Voice Capture
The browser microphone records the user’s voice input for a fixed duration.

Audio Conversion
The recorded audio is converted from the browser format into a high-quality .wav file using FFmpeg.

Speech-to-Text (STT)
The audio file is transcribed into text using Google’s Web Speech API in the selected language.

LLM Processing

The transcribed text is sent to the Google Gemini LLM.

The model analyzes intent and context and generates a response in the same language.

Text-to-Speech (TTS)
The generated response is converted into speech using Google Text-to-Speech.

Spoken Output
The final audio response is played back to the user.

### Getting Started
## Prerequisites

A Google account (for Google Colab)

A Google Gemini API key (available from Google AI Studio)

## Installation and Usage

Open the Notebook

Click the “Open in Colab” badge, or

Visit colab.research.google.com and upload the notebook file.

Add API Key

In the first code cell, paste your Gemini API key into the API_KEY variable.

Run the Notebook

Select Runtime → Restart and run all.

Grant Microphone Access

Allow microphone access when prompted by the browser.

Interact with the Assistant

Click Start Listening and speak in the active language (default: Tamil).

Click Switch Language to toggle between Tamil and English.

## Technologies Used

Programming Language: Python

Environment: Google Colab

Large Language Model: Google Gemini 1.5 Flash

Speech-to-Text: SpeechRecognition library (Google Web Speech API)

Text-to-Speech: gTTS (Google Text-to-Speech)

Audio Processing: FFmpeg

## Future Improvements

Wake-word detection for fully hands-free activation.

Conversational memory to support multi-turn dialogue.

Integration with external APIs (e.g., weather, news, real-time data).

Standalone web deployment using Flask or Streamlit.
