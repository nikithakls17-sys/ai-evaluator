AI Evaluator



AI Evaluator is a Python-based interactive tutor designed to assess a student’s understanding of various topics through adaptive questioning. It uses OpenAI’s GPT model to generate dynamic questions, evaluate responses, and provide feedback on the learner’s knowledge level.



Project Overview



The project simulates an AI tutor that:



Asks progressively challenging questions about a chosen topic.



Evaluates user responses to determine their understanding level.



Provides a final summary with strengths, weaknesses, and learning recommendations.



Uses a persistent SQLite memory system to store session progress.



Features



Adaptive question-based evaluation



Topic-specific rubric generation



Suggested subtopics for deeper learning



Persistent session management using SQLite



Configurable through environment variables



Modular code structure for easy expansion



Technologies Used



Python 3.13



OpenAI API (GPT-3.5-Turbo)



openai-agents



SQLite for session persistence



dotenv for environment variable handling



uv for environment and dependency management



Setup Instructions

1\. Clone the repository

git clone https://github.com/nikithakls17-sys/ai-evaluator.git

cd ai-evaluator



2\. Create and activate a virtual environment

uv venv



3\. Install dependencies

uv sync



4\. Create a .env file



Create a file named .env in the root directory and add the following:



OPENAI\_API\_KEY=your\_openai\_api\_key\_here

MODEL\_ID=gpt-3.5-turbo



5\. Run the program

uv run main.py



How It Works



Session Initialization

A SQLite session database (memory.db) is created to store user input and progress.



Question Flow

The AI begins with basic questions and gradually increases difficulty based on user responses.



Diagnostic Tools



get\_diagnostic\_rubric(topic) generates a rubric from beginner to advanced levels.



suggest\_subtopics(topic) lists subtopics for continued learning.



Final Evaluation

The agent summarizes the learner’s comprehension level, identifies gaps, and suggests improvement areas.



Development Process



Set up a Python 3.13 virtual environment using uv.



Installed and configured required dependencies in pyproject.toml.



Created function tools for topic evaluation and rubric generation.



Integrated the OpenAI API and configured access through environment variables.



Implemented persistent session management using SQLite.



Tested multiple API configurations (OpenRouter, OpenAI) to ensure stability.



Successfully deployed the working version and pushed it to GitHub.



Project Status



The project is fully functional using OpenAI API.



Successfully verified model operation and responses.



Uploaded to GitHub for further development and integration.



Next step: Extend this AI system into the UCMO Symposium project as an Admissions Chatbot to assist incoming students with the application process.



Author



Nikitha Kishore Avadootha

University of Central Missouri

AI Evaluator Project – 2025

