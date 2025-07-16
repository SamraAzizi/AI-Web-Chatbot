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
├── flaskApp/ # Production Flask app
│ ├── model/ # Deployed model files
│ │ ├── chatbotModel.keras # Trained neural network
│ │ ├── classes.pkl # Response categories
│ │ └── words.pkl # Vocabulary mappings
│ ├── templates/
│ │ └── index.html # Web interface
│ ├── app.py # Main application
│ └── utils.py # Support functions
├── preparations/ # Development area
│ ├── model/ # Training artifacts
│ │ ├── chatbotModel.keras
│ │ ├── classes.pkl
│ │ └── words.pkl
│ ├── chatbot.py # Core logic
│ ├── intents.json # Training data
│ └── modelTraining.py # Model builder
├── .env # Configuration
├── venv/ # Python environment
└── README.md # Documentation
```