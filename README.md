📘 Career Conversation Chatbot (AI Digital Twin)
Gemini-Powered Career Chatbot Deployed on Hugging Face

An AI-powered career chatbot that acts as my professional digital twin.
It answers questions based on my LinkedIn profile and career summary, engages visitors like a real conversation, and intelligently captures leads.

🔗 Live Demo:https://huggingface.co/spaces/ypawar6921/career_conversation

🚀 Overview

This project transforms a static resume into an interactive AI experience.

The chatbot:
-Responds to career and background questions

-Stays strictly in character

-Captures user contact details

-Logs unanswered questions for improvement

-Sends real-time notifications

Built using:
Google Gemini API,
OpenAI-compatible SDK,
Function calling,
Gradio UI,
Hugging Face deployment

🧠 How It Works
1️⃣ Context-Based Intelligence
The system prompt dynamically injects:
Extracted text from Linkedin.pdf
Content from Summary.txt
This ensures responses are grounded in real professional information.

2️⃣ Function Calling (Tool Usage)

The chatbot uses structured tools for controlled actions.
🔹 record_user_details
Triggered when a visitor shares their email or expresses interest.

Parameters:
email (required),
name (optional),
notes (optional)

Sends a real-time notification via Pushover.

🔹 record_unknown_question
Triggered when the chatbot cannot answer a question.

This helps:
Identify knowledge gaps.
Improve future versions..
Track unexpected user queries

3️⃣ Notification Layer

Uses the Pushover API to send instant alerts when:
A user shares contact information,
An unknown question is asked

🌍 Deployment

This chatbot is deployed on Hugging Face Spaces, making it accessible publicly through a live URL.

To deploy:
Create a new Space (Gradio template)
Upload project files
Add environment variables in Space settings
Set app.py as the entry file
