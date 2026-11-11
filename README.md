# 🤖 HFAssist — Multimodal AI Assistant

HFAssist is a multimodal AI project that brings together Text, Image, Audio, and Video processing using Hugging Face Transformers and a Telegram Bot interface.

The project provides multiple AI-powered capabilities through individual pipelines and makes selected features accessible through a single Telegram bot.

## 🚀 Project Overview

HFAssist consists of four major AI pipelines:

### 1. 📝 Text Pipeline
Performs different Natural Language Processing (NLP) tasks.

**Features:**
- Sentiment Analysis
- Text Summarization
- Text Generation
- Language Translation (English to French)
- Zero-Shot Classification

**Models Used:**
- `distilbert/distilbert-base-uncased-finetuned-sst-2-english`
- `facebook/bart-large-cnn`
- `distilgpt2`
- `Helsinki-NLP/opus-mt-en-fr`
- `facebook/bart-large-mnli`

### 2. 🖼️ Image Pipeline
Processes images using computer vision models.

**Features:**
- Image Classification
- Object Detection
- Image Captioning

**Models Used:**
- `google/vit-base-patch16-224`
- `facebook/detr-resnet-50`
- `nlpconnect/vit-gpt2-image-captioning`

### 3. 🎙️ Audio Pipeline
Converts spoken audio into text using Automatic Speech Recognition (ASR).

**Feature:**
- Audio-to-Text Transcription

**Model Used:**
- `openai/whisper-tiny`

### 4. 🎬 Video Pipeline
Analyzes video content using a video classification model.

**Feature:**
- Video Classification

**Model Used:**
- `MCG-NJU/videomae-base-finetuned-kinetics`

## 📱 Telegram Bot Integration

HFAssist integrates selected pipeline features into a single Telegram bot, allowing users to interact with AI models directly through Telegram.

**Available Commands:**

| Command | Function |
|---|---|
| `/start` | Start the bot |
| `/sentiment` | Analyze text sentiment |
| `/summarize` | Summarize text |
| `/translate` | Translate English to French |
| `/generate` | Generate text |

**Additional Features:**
- Send an image for image classification.
- Send a voice message or audio file for transcription.
- Send a video for video classification.

## 🛠️ Technologies Used

- Python
- Hugging Face Transformers
- PyTorch
- OpenCV
- Whisper
- VideoMAE
- python-telegram-bot
- Google Colab

## 📂 Project Structure

```text
HFAssist/
│
├── text_pipeline.ipynb
├── image_pipeline.ipynb
├── vid_pipeline.ipynb
├── HFAssist_Telegram_Bot.ipynb
│
├── requirements.txt
├── README.md
│
├── Documentation/
├── Screenshots/
└── Demo/
```

## ⚙️ Installation and Setup

**1. Clone the repository**

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

**2. Navigate to the project directory**

```bash
cd HFAssist
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Open the notebooks**

Open the required `.ipynb` files using Google Colab or Jupyter Notebook.

**5. Configure Telegram Bot**

- Create a Telegram bot using BotFather.
- Obtain your bot token.
- Store the token securely using an environment variable.
- Run the Telegram bot notebook and interact with your bot.

**Note:** Never upload your Telegram bot token or other secret credentials to GitHub.

## 📊 Project Results

The individual pipelines were implemented and tested in their respective notebooks.

Selected features were also integrated and tested through the Telegram bot:

- Text Processing — Successfully tested
- Image Classification — Successfully tested
- Audio Transcription — Successfully tested
- Video Classification — Successfully tested

## ⚠️ Limitations

- The Telegram bot runs through the active notebook runtime and requires the runtime to remain connected.
- VideoMAE is trained on action-recognition categories, so its predictions may not accurately describe specialized content such as medical videos.
- Not every task implemented in the individual notebooks is currently available through Telegram.

## 🎯 Project Objective

The main objective of HFAssist is to explore and integrate multiple AI modalities into one unified system, demonstrating how different Hugging Face models can be combined to build practical AI-powered applications.

---

**HFAssist — Bringing Multiple AI Capabilities Together in One Assistant.** 🤖
