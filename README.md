eb0a1969249b9ca67802dca16d3dd05def0083d7# InstantLegal AI - Legal Document Generator

A Flask web application that generates professional legal documents using OpenAI's GPT-4 API and ReportLab for PDF generation.

## Features

- AI-powered legal document generation
- Multiple document types (NDA, Terms of Service, Privacy Policy, etc.)
- Customization based on business type, industry, and state
- PDF generation and download
- Responsive web interface

## Tech Stack

- **Backend**: Python 3.10+, Flask
- **AI**: OpenAI GPT-4 API
- **PDF Generation**: ReportLab
- **Frontend**: HTML, CSS, JavaScript (Vanilla)
- **Security**: Flask-Limiter for rate limiting, CORS protection

## Installation

1. Clone the repository:
```
git clone <repository-url>
cd instantlegal-ai
```

2. Create a virtual environment and activate it:
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```
pip install -r requirements.txt
```

4. Create a `.env` file in the root directory with the following variables:
```
FLASK_APP=app.py
FLASK_ENV=development
OPENAI_API_KEY=your_openai_api_key_here
SECRET_KEY=your_secret_key_here
```

5. Run the application:
```
flask run
```

6. Open your browser and navigate to `http://localhost:5000`

## Usage

1. Select a document type from the dropdown menu
2. Fill in your business details
3. Choose protection level and any special clauses
4. Click "Generate Document Now"
5. Download your generated PDF document

## Project Structure

```
instantlegal-ai/
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (not in repo)
├── .gitignore              # Git ignore file
├── README.md               # Project documentation
├── static/                 # Static files
│   ├── css/                # CSS files
│   ├── js/                 # JavaScript files
│   └── documents/          # Generated documents
└── templates/              # HTML templates
    └── index.html          # Main application template
```

## License

MIT

## Disclaimer

This application is for demonstration purposes only. The generated legal documents should be reviewed by a qualified legal professional before use in a real-world context. 