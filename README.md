# AI Chatbot for Students 🤖

## 📌 Overview
A simple chatbot built in Python to answer frequently asked questions by students.  
It uses basic NLP techniques to provide responses.

## 🔧 Tools & Technologies
- Python
- NLTK / spaCy
- Flask (for web deployment)

## 🚀 Features
- Answer FAQs for students
- Easy to expand with more intents
- Can be integrated into web or mobile apps

## 📂 How to Run
```bash
python chatbot.py
```
# AI Chatbot for Students 🤖
# Basic chatbot using Python dictionaries (extend with NLP libraries)

def chatbot_response(user_input):
    responses = {
        "hi": "Hello! How can I help you today?",
        "bye": "Goodbye! Have a nice day.",
        "who are you": "I am a simple student chatbot.",
    }
    return responses.get(user_input.lower(), "Sorry, I don't understand that yet.")

if __name__ == "__main__":
    print("Chatbot is running... (type 'bye' to exit)")
    while True:
        user_input = input("You: ")
        response = chatbot_response(user_input)
        print("Bot:", response)
        if user_input.lower() == "bye":
            break
