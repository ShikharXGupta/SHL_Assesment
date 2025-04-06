# SHL Audio Assessment: Transcription and Grammar Scoring

This notebook is designed for scoring spoken English responses in SHL-style assessments. It transcribes audio using OpenAI's Whisper and evaluates the grammar of the transcribed text using a rule-based checker — **without using any ML models**.

---

## 📌 Features

- 🎙 Upload and play audio (mp3, wav, m4a)
- 🗣 Transcribe audio to text using Whisper
- ✍️ Rule-based grammar checking (no ML models)
- 🧠 Automatic scoring out of 10
- 📋 Displays grammar suggestions and error types

---

## 📦 Requirements

Run the following in a notebook cell to install the required libraries:

```python
# Install Git if missing (for Colab)
!apt-get install git -y

# Install libraries
!pip install -q git+https://github.com/openai/whisper.git
!pip install -q torchaudio
!pip install -q pydub
!pip install -q language-tool-python

