🧠 Auto Tagging Support Tickets Using LLM
📌 Overview

This project demonstrates how to automatically categorize customer support tickets into relevant topics using a Large Language Model (LLM).
Instead of traditional training, it leverages zero-shot classification to tag tickets based on plain-text category names.
This approach allows fast deployment of intelligent support systems without the need for labeled data.

🎯 Objectives

Build a zero-shot ticket classifier using facebook/bart-large-mnli

Automatically tag support requests into relevant categories

Evaluate performance using confidence scores

Deploy an interactive Gradio app for real-time testing

🛠️ Tech Stack

Python 3

Hugging Face Transformers – zero-shot classification pipeline

PyTorch – model backend

Gradio – web-based demo interface

📂 Repository Structure
├── Task3_AutoTagging_LLM.ipynb   # Colab notebook (main implementation)
├── README.md                      # This documentation file

⚡ How to Run
1️⃣ Install Dependencies
pip install -q transformers torch gradio

2️⃣ Open the Notebook

Run the notebook Task3_AutoTagging_LLM.ipynb in Google Colab (GPU not required).

3️⃣ Run the Cells

The notebook will:

Initialize a zero-shot classification model

Define candidate ticket labels

Predict tags for input text

Launch a Gradio demo for interactive use

🧩 Example Usage

Input:

I was charged twice for my monthly plan and need a refund.


Output:

Predicted Tag: Billing Issue (Confidence: 0.94)


Candidate Labels:

Billing Issue

Technical Problem

Account Management

Service Outage

General Inquiry

Feature Request

✨ Features

✅ Zero-shot classification (no training required)

⚡ Fast and lightweight deployment

🌐 Interactive Gradio interface

🔁 Easily adaptable to custom categories

📊 Results Summary
Example Ticket	Predicted Tag	Confidence
“App keeps crashing after update.”	Technical Problem	0.88
“My payment was deducted twice.”	Billing Issue	0.94
“Please add dark mode feature.”	Feature Request	0.89
📌 Author

Developed as part of the AI/ML Engineering Advanced Internship by DevelopersHub Corporation
