#  AI Web Chatbot  
*Flask-based chatbot with custom model training and OpenAI integration*

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Flask](https://img.shields.io/badge/Flask-2.0%2B-lightgrey)
![OpenAI](https://img.shields.io/badge/OpenAI-gpt--3.5%2B-brightgreen)

##  Project Structure

##  Table of Contents
- [Features](#-features)
- [Installation](#-installation)
- [Configuration](#-configuration)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Deployment](#-deployment)
- [Troubleshooting](#-troubleshooting)
- [License](#-license)

##  Features
- Web-based ChatGPT interface
- Session history management
- Responsive design
- Easy OpenAI API integration

##  Installation

### Prerequisites
- Python 3.8+
- OpenAI API key
- Git (optional)

### Steps
1. Clone the repository:
   ```bash
   git https://github.com/SamraAzizi/AI-Web-Chatbot.git
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
   FLASK_APP=flaskApp/app.py
   FLASK_ENV=development
   ```
5. Run the application:
   ```bash
   python flaskApp/app.py
   ```
   
## Configuration

Edit app.py to customize:
   ```bash
   # Change model (default: gpt-3.5-turbo)
   model = "gpt-3.5-turbo"  

   # Modify temperature (0-2)
   temperature = 0.7
   ```

## Usage
Run the application:

```bash
python app.py
```

Then open http://localhost:5000 in your browser.

## Project Structure
```bash
AI-Web-Chatbot/
├── flaskApp/ # Main Flask application
│ ├── model/ # Trained model files
│ ├── templates/ # Frontend templates
│ │ └── index.html # Chat interface
│ ├── app.py # Flask application entry
│ └── utils.py # Helper functions
├── preparations/ # Training and data preparation
│ ├── model/ # Model training files
│ ├── chatbot.py # Core chatbot logic
│ ├── intents.json # Training data
│ └── modelTraining.py # Model training script
├── .env # Environment variables
├── venv/ # Virtual environment
└── README.md # This file
```