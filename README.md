# AI Email Classification & Reply Assistant

A Python-based application that classifies emails, detects priority, summarizes email content, and generates editable reply drafts.

## Features

- Email classification into Finance, Scheduling, Support, and General categories
- Priority detection: Urgent, Important, and General
- Automatic email summarization
- Professional reply draft generation
- Editable reply drafts with text-file download
- Rule-based analysis with optional OpenAI API integration
- Interactive Streamlit interface

## Technologies Used

- Python
- Streamlit
- OpenAI API
- JSON
- Rule-based text processing

## Installation

1. Clone the repository.
2. Install the dependencies:

   `python -m pip install -r requirements.txt`

3. Start the application:

   `python -m streamlit run app.py`

4. Open the local URL displayed in the terminal.

## AI Integration

The application supports optional OpenAI API integration. Without an API key, it uses rule-based classification and predefined reply templates.

To enable the OpenAI integration, configure the `OPENAI_API_KEY` environment variable. Never commit API keys to GitHub.

## Limitations

- Rule-based classification depends on predefined keywords.
- Summaries in fallback mode use the first two sentences.
- Suggested replies must be reviewed before use.
- The application does not send emails automatically.