#Cloud-Based-YouTube-Video-Transcription-and-NLP-Summarization

##Overview

Cloud-Based-YouTube-Video-Transcription-and-NLP-Summarization is an end-to-end web application developed to automate the process of extracting audio from YouTube videos, transcribing speech using Google Cloud Speech-to-Text API, and generating concise summaries using Natural Language Processing techniques.

The project demonstrates practical implementation of cloud computing, speech recognition, and NLP within a scalable web-based architecture. It integrates multiple technologies to provide an efficient solution for automated video content analysis.

Objective

The objective of this project is to design and implement a cloud-enabled system capable of accurately transcribing spoken video content and generating meaningful summaries, enabling faster information extraction and improved accessibility.

Key Features

Extraction of audio from YouTube videos using yt-dlp

Upload of audio files to Google Cloud Storage

Speech transcription using Google Cloud Speech-to-Text API

Extractive text summarization using spaCy

Web-based interface developed with Flask

Fully automated end-to-end processing workflow

System Workflow

The user provides a YouTube video URL through the web interface.

The application downloads and extracts the audio from the video.

The audio file is uploaded to Google Cloud Storage.

Google Cloud Speech-to-Text processes the audio and generates a transcription.

The transcription is analyzed using NLP techniques to produce a summary.

The transcription and summary are displayed to the user.

Technologies Used

Python

Flask

Google Cloud Speech-to-Text API

Google Cloud Storage

spaCy

yt-dlp

HTML and CSS

Installation and Setup
Clone the Repository

git clone https://github.com/Divya-Sri-Lingala/Cloud-Based-YouTube-Video-Transcription-and-NLP-Summarization.git

cd Cloud-Based-YouTube-Video-Transcription-and-NLP-Summarization

Configure Google Cloud

Create a Google Cloud account.

Enable the Speech-to-Text API.

Download the service account credentials JSON file.

Set the environment variable:

On macOS or Linux:

export GOOGLE_APPLICATION_CREDENTIALS="path_to_your_credentials_file.json"

On Windows:

set GOOGLE_APPLICATION_CREDENTIALS=path_to_your_credentials_file.json

Install Dependencies

python -m venv venv
source venv/bin/activate
pip install -r requirements.txt

On Windows:

venv\Scripts\activate

Run the Application

python app.py

Access the application at:

http://127.0.0.1:5000/

Project Structure

app.py – Main Flask application
processing.py – Core logic for downloading, transcribing, and summarizing
templates/index.html – Homepage template
templates/result.html – Results page template
static/style.css – Styling file
requirements.txt – Project dependencies
README.md – Documentation
LICENSE – License information

Future Enhancements

Deployment on cloud platforms such as AWS or GCP

Support for multilingual transcription

Integration of transformer-based summarization models

User authentication and transcript storage

License

This project is licensed under the MIT License.
