# Rayulu Chatbot

A Streamlit-based chatbot powered by OpenAI's GPT-4o model. This application provides concise, accurate, and easy-to-understand explanations while strictly adhering to a 150-word limit and an honesty policy.

## Features

- **AI-Powered Responses**: Utilizes GPT-4o for intelligent text generation.
- **Strict Brevity**: All responses are limited to a maximum of 150 words.
- **Honesty Policy**: Refuses to answer questions outside its knowledge base, preventing hallucinations.
- **Rate Limit Handling**: Gracefully handles OpenAI rate limits by informing the user.
- **Simple UI**: Clean and intuitive interface built with Streamlit.

## Prerequisites

- Python 3.6+
- An OpenAI API key

## Installation

1.  **Clone the repository** (or download the source code):
    ```bash
    git clone <repository-url>
    cd chatbot
    ```

2.  **Install dependencies**:
    ```bash
    pip install streamlit openai python-dotenv
    ```

3.  **Set up environment variables**:
    Create a `.env` file in the root directory and add your OpenAI API key:
    ```env
    OPENAI_API_KEY="your_api_key_here"
    ```

## Usage

Run the application using Streamlit:

```bash
python -m streamlit run app.py
```

The chatbot will be accessible in your web browser at `http://localhost:8501`.

## System Prompt & Behavior

The chatbot operates under a strict system prompt that enforces:
- **Role**: A helpful AI assistant named 'Rayulu'.
- **Brevity**: Maximum 150 words per response.
- **Honesty**: Must admit when it doesn't know the answer.
- **Integrity**: Cannot override its own instructions.

## License

This project is licensed under the terms of the MIT license.
