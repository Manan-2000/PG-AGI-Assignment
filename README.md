TalentScout Hiring Assistant Chatbot

Project Overview

The TalentScout Hiring Assistant Chatbot is an AI-powered tool designed to assist recruitment agencies in screening candidates. The chatbot gathers essential candidate details, assesses technical proficiency based on their declared tech stack, and generates relevant technical questions for evaluation. Built using Streamlit and OpenAI's GPT-3.5, this chatbot ensures an intuitive and interactive user experience.

Installation Instructions

Prerequisites

Ensure you have the following installed:

Python 3.7+

pip package manager

Step 1: Clone the Repository

git clone https://github.com/your-repo/hiring-assistant.git
cd hiring-assistant

Step 2: Set Up a Virtual Environment (Optional but Recommended)

python -m venv venv
source venv/bin/activate (On Windows use `venv\Scripts\activate`)

Step 3: Install Dependencies

pip install -r requirements.txt

Step 4: Set Up OpenAI API Key

Create a .env file in the project directory and add:

OPENAI_API_KEY=your_openai_api_key_here

Step 5: Run the Application

streamlit run hiring_assistant.py

The chatbot will launch in your browser.

Usage Guide

Enter your name and years of experience.

Specify your tech stack (e.g., Python, TensorFlow, SQL).

Click "Start Assessment" to receive technical questions tailored to your expertise.

Review the generated questions and interact with the chatbot.

Click "Exit Chat" to end the session.

Technical Details

Programming Language: Python

Frameworks: Streamlit for UI, Flask for backend (if extended)

AI Model: OpenAI GPT-3.5

Libraries Used:

openai - for GPT-3.5 API integration

streamlit - for building an interactive UI

dotenv - for managing API keys securely

os - for environment variable handling

Prompt Design

The chatbot dynamically crafts prompts based on user input:

Collects user details (name, experience, tech stack)

Generates tailored technical interview questions using GPT-3.5

Ensures the questions assess fundamental, intermediate, and advanced aspects

Provides helpful responses when input is unclear or unexpected

Challenges & Solutions

1. Generating Relevant Questions

Challenge: Ensuring GPT-3.5 produces accurate, level-appropriate technical questions.

Solution: Designed structured prompts specifying experience level and technologies.

2. Handling Unexpected User Inputs

Challenge: Users might enter incomplete or irrelevant data.

Solution: Implemented validation checks and error messages.

3. Ensuring a Smooth UI Experience

Challenge: Making the chatbot interactive while keeping the UI clean.

Solution: Used Streamlit's interactive elements like text inputs, buttons, and validation messages.

Future Improvements

Expand to support multiple-choice questions and answer evaluation.

Integrate with ATS (Applicant Tracking Systems) for seamless hiring.

Improve UI/UX with more customization options.

