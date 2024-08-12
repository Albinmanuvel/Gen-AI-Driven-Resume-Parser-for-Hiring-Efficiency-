# Flask-Resume-Parser-Application


This is a Flask-based web application that allows users to upload resumes in PDF format. It extracts text from the PDFs, parses key information using OpenAI's GPT-4 model, and stores the data in an SQLite database.

## Features

- **Upload Resumes**: Upload resumes in PDF format.
- **Extract Text**: Extract text from uploaded PDFs.
- **Parse Data**: Use OpenAI's GPT-4 to parse the text and extract structured information.
- **Store Data**: Save parsed resume data in an SQLite database.
- **View Resumes**: View a list of uploaded resumes and their details.

## Requirements

- Python 3.x
- Flask
- Flask-SQLAlchemy
- PyPDF2
- OpenAI Python client

# Create and Activate a Virtual Environment:

python -m venv venv
source venv/bin/activate  

On Windows use `venv\Scripts\activate`

# Install Dependencies:

pip install Flask Flask-SQLAlchemy PyPDF2 openai

Set OpenAI API Key:

export OPENAI_API_KEY='your_api_key_here'  

 On Windows use `set OPENAI_API_KEY='your_api_key_here'`


## Usage
Run the Application :

python app.py
Access the Application :

Open your web browser and go to http://127.0.0.1:5000/.

Upload and View Resumes:

Use the upload form to upload a PDF resume.
Navigate to /resumes to view all resumes and their details.
Application Structure
app.py: Main Flask application file.
models.py: Contains database models.
templates/: HTML templates for the web pages.
uploads/: Directory for storing uploaded resumes.