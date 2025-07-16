# 🤖 AI Web Chatbot  
*A Flask-based web interface for OpenAI's ChatGPT API*

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![Flask Version](https://img.shields.io/badge/flask-2.0%2B-lightgrey)
![OpenAI](https://img.shields.io/badge/OpenAI-gpt--3.5%2B-brightgreen)

## 📌 Table of Contents
- [Features](#-features)
- [Installation](#-installation)
- [Configuration](#-configuration)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Deployment](#-deployment)
- [Troubleshooting](#-troubleshooting)
- [License](#-license)

## ✨ Features
- Web-based ChatGPT interface
- Session history management
- Responsive design
- Easy OpenAI API integration

## 💻 Installation

### Prerequisites
- Python 3.8+
- OpenAI API key
- Git (optional)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/SamraAzizi/AI-Web-Chatbot.git
   cd AI-Web-Chatbot
   ```

2. Create and activate virtual environment:
   ```bash
   python -m venv venv
   # Windows:
   venv\Scripts\activate
   # Mac/Linux:
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Create .env file:
   ```bash
   OPENAI_API_KEY=your_api_key_here
   ```

## Configuration

Edit app.py to customize:
   ```bash
   # Change model (default: gpt-3.5-turbo)
   model = "gpt-3.5-turbo"  

   # Modify temperature (0-2)
   temperature = 0.7
   ```
   
