# Vibe Check

A Django web app that analyzes the sentiment of YouTube video comments. Paste a YouTube URL and get a breakdown of how the audience feels — positive, negative, or neutral — along with a word cloud and language distribution.

## Features

- Sentiment analysis of up to 800 YouTube comments
- Word cloud visualization
- Language distribution of comments
- Contact/feedback form

## Tech Stack

- Python, Django
- YouTube Data API v3
- TextBlob (sentiment analysis)
- WordCloud, LangDetect, Pandas

## Setup

1. Clone the repo and install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Add your YouTube Data API key in `checkvibe/views.py`:
   ```python
   api_key = "YOUR_API_KEY"
   ```

3. Run migrations and start the server:
   ```bash
   python manage.py migrate
   python manage.py runserver
   ```

## Getting a YouTube API Key

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a project and enable **YouTube Data API v3**
3. Generate an API key under **Credentials**
