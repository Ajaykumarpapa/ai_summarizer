# AI Document Summarizer

Transform lengthy documents into concise, intelligent summaries using advanced NLP techniques. Supports both extractive (key sentence selection) and abstractive (AI-generated) summarization methods.

## Features

- **Text Input**: Paste any text directly for summarization
- **URL Input**: Extract and summarize content from any webpage using BeautifulSoup
- **PDF Upload**: Upload PDF files for text extraction and summarization
- **Extractive Summarization**: Selects key sentences from original text using spaCy and TF-IDF scoring
- **Abstractive Summarization**: Generates new AI-powered summaries using Facebook's BART model (bart-large-cnn)
- **Detail Levels**: Choose between Beginner, Intermediate, or Expert summaries with adjustable output length
- **Real-time Metrics**: Displays original length, summary length, compression ratio, and processing time

## Technologies Used

- **Streamlit** - Web application framework
- **spaCy** (en_core_web_sm) - Natural language processing for extractive summarization
- **Transformers** (BART) - AI-powered abstractive summarization via Hugging Face
- **PyTorch** - Deep learning backend for transformer models
- **BeautifulSoup** - Web scraping and HTML content extraction
- **PyPDF2** - PDF text extraction
- **requests** - HTTP client for URL fetching

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```bash
streamlit run summarizer.py
```

The application will open in your browser at `http://localhost:8501`.

### Configuration Options

- **Input Method**: Text / URL / PDF
- **Summarization Method**: Extractive or Abstractive
- **Detail Level**: Beginner (shorter), Intermediate (balanced), Expert (detailed)
- **Number of Sentences**: Adjustable for extractive mode (1-10)

## Project Structure

```
.
├── summarizer.py       # Main Streamlit application (297 lines)
├── requirements.txt    # Python dependencies with pinned versions
├── packages.txt        # System-level dependencies (python3-dev, build-essential)
├── gitignore           # Git ignore configuration
└── readme.md           # Project documentation
```

## Deployment

This app is compatible with Streamlit Cloud deployment.

## License

MIT License
