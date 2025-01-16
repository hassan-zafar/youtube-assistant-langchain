# YouTube Assistant

![YouTube Assistant](<YouTube-Assistant.png>) <!-- Replace <image-url-here> with the actual image URL -->

YouTube Assistant is a web application that answers questions about YouTube videos by analyzing their transcripts. Built using Streamlit, LangChain, and OpenAI, this tool allows users to input a YouTube video URL and ask questions about its content.

## Features

- Extracts and processes YouTube video transcripts
- Splits large transcripts into manageable chunks for analysis
- Performs semantic search using FAISS to find relevant transcript sections
- Uses OpenAI's GPT models to provide detailed answers
- Dark theme UI with purple accent colors

## Prerequisites

- Python 3.9+
- OpenAI API key

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd youtube-assistant
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**:
   ```bash
   streamlit run main.py
   ```

## Docker Support

You can also run the application using Docker:

```bash
docker build -t youtube-assistant .
docker run -p 8501:8501 youtube-assistant
```

## Usage

1. Access the application through your web browser at `http://localhost:8501`
2. In the sidebar:
   - Enter a YouTube video URL
   - Type your question about the video
   - Provide your OpenAI API key
3. Click Submit to get your answer

## Dependencies

- python-dotenv
- langchain
- openai
- youtube-transcript-api
- faiss-cpu
- streamlit

## Environment Configuration

The application uses a dark theme by default, which is configured in `.streamlit/config.toml`.

## Security Note

- The application requires an OpenAI API key
- API keys are handled securely and are not stored
- The `.env` file is excluded from version control

## Contributing

Feel free to submit issues and enhancement requests.


