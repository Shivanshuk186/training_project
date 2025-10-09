# training_project
🤖 Simple PDF Q&A Chatbot
<p align="center">

<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow"/>


</p>

A command-line chatbot that answers questions based on the content of multiple PDF files using a keyword-matching algorithm.

📋 Table of Contents
📖 Description

✨ Features

⚙️ How It Works

🛠️ Requirements

🚀 Setup and Usage

💡 Example

📖 Description
This project is a command-line chatbot that answers questions based on the content of multiple PDF files. It extracts text from all PDFs in a specified folder, uses a keyword-matching algorithm to find the most relevant sentences related to a user's query, and synthesizes them into a concise answer.

The script also builds a simple Deep Neural Network (DNN) and a Linear Regression model for demonstration purposes, but the core answering mechanism relies on a direct keyword search for simplicity and speed.

✨ Features
📁 Text Extraction: Automatically reads and extracts text from all PDF files placed in a pdfs folder.

🔍 Keyword Search: Ranks sentences from the documents based on how many keywords they share with the user's question.

📝 Concise Answers: Combines the most relevant sentences to generate a summary answer of approximately 100 words.

💻 Interactive Interface: Simple and easy-to-use command-line interface for asking questions.

⚙️ How It Works
PDF Reading: The script first scans the pdfs directory and reads all text content from the .pdf files.

Text Processing: The extracted text is cleaned and split into individual sentences.

Model Training: A basic DNN and a Linear Regression model are trained on the sentence data.

User Query: The chatbot prompts the user for a question.

Scoring: It calculates a relevance score for each sentence by counting the number of matching keywords from the user's query.

Answer Generation: The sentences with the highest scores are sorted, and their text is combined to form the final answer, which is then displayed to the user.

🛠️ Requirements
You will need to have Python installed, along with the following libraries:

PyPDF2

numpy

scikit-learn

tensorflow

You can install them all using pip:

pip install PyPDF2 numpy scikit-learn tensorflow

🚀 Setup and Usage
Prepare Your Files:

Create a folder named pdfs in the same directory as the script.

Place all the PDF files you want the chatbot to learn from inside this pdfs folder.

Run the Script:

Open a terminal or command prompt.

Navigate to the project directory.

Run the script using the following command:

python project.py

(Note: If you are running it from the Jupyter Notebook, simply execute the cell.)

Interact with the Chatbot:

Wait for the "Reading PDFs..." and "Training models..." messages to complete.

Once you see Chatbot ready!, you can start asking questions.

Type your question and press Enter.

To stop the chatbot, type exit and press Enter.

💡 Example
You: what is the software development life cycle?

Chatbot:
sdlc models software development life cycle (sdlc) is a spiritual model used in project management that defines the stages include in an information system development project, from an initial feasibility study to the maintenance of the completed application. the stages of sdlc are as follows: stage1: planning and requirement analysis requirement analysis is the most important and necessary stage in sdlc. when to use sdlc waterfall model? here, are some important phases of sdlc life cycle: waterfall model the waterfall is a universally accepted sdlc model. need of sdlc the development team must determine a suitable life cycle model for...

--------------------------------------------------------------------------------
