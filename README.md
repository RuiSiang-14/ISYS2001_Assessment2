# ISYS2001_Assessment2  Smart Personal Budget Assistant

1.Project Overview

This project is called Smart Personal Budget Assistant. It is a Python program that helps university students manage their money.
The program allows users to enter their monthly income, upload their expense CSV file, and check how much money they have spent and how much they have left.
I also used Google Gemini AI to create a chatbot that can give some advice about budgeting and saving money.

2.Project Objectives

The main purpose of this project is to help students understand their spending and manage their money better.

The program can:

1. Calculate total monthly expenses.
2. Calculate the remaining money after expenses.
3. Show the percentage of income spent.
4. Find which expense category costs the most.
5. Give budgeting advice using Gemini AI.

3.Main Features

Budget Calculation:
The program calculates the user's total expenses, remaining balance, and spending percentage.

CSV File Upload:
Users can upload a CSV file that contains their expenses. The program will read the file using pandas.

Gemini AI Chatbot:
The chatbot can answer questions about budgeting and saving money. It also uses the user's financial information to give more suitable advice.

Gradio Interface
I used Gradio to create a simple interface so users can enter their information and use the program without writing Python code.

Error Handling
I added some error handling to prevent the program from crashing when users enter incorrect information or when Gemini is temporarily unavailable.

4.Technologies Used

| Technology | Purpose|
|---|---|
| Python | Used to write the program |
| pandas | Used to read and analyse CSV files |
| Google Gemini API | Used to create the finance chatbot |
| Gradio | Used to create the user interface |
| GitHub Codespaces | Used to develop and save the project |

5.How to Run the Program

1. Open ISYS2001 Finance_Assisstant.ipynb
2. Install the required Python libraries: pandas, google-genai and gradio.
3. Get a Gemini API key from Google AI Studio.
4. Run the API key cell and enter the key.
5. Run the notebook cells in order.
6. Run the Gradio interface code.
7. Open the Gradio application.
8. Enter your monthly income.
9. Upload your expense CSV file.
10. Enter a question about budgeting.
11. Click Analyse My Budget to see the result.

6.CSV File Format

The CSV file needs to have four columns: Date, Description, Category and Amount.

Example:

| Date | Description | Category | Amount |
|---|---|---|---|
| 2026-10-01 | Monthly rent | Rent | 1000 |
| 2026-10-03 | Groceries | Food | 500 |
| 2026-10-05 | Bus fares | Transport | 200 |
| 2026-10-07 | Movies | Entertainment | 300 |

7.Example Budget Result

For example, if a student earns AUD 3,000 per month and has AUD 2,000 in expenses, the program will calculate:

- Monthly income: AUD 3,000
- Total expenses: AUD 2,000
- Remaining balance: AUD 1,000
- Spending percentage: 66.67%
- Highest expense category: Rent

The student can also ask Gemini questions such as "How can I reduce my spending?"

8.Testing and Debugging

I used assert o test some of the Python functions. The tests include calculating total expenses, remaining balance, spending percentage, and finding the largest expense category.

I also tested some special cases such as zero income, empty expenses, and spending more than the monthly income.

During development, I faced some problems. One of the problems was the Gemini API showing a 503 UNAVAILABLE error because the model was too busy.

To solve this problem, I added try and except to handle the error. I also added a retry function so the chatbot can try again when Gemini is busy.

9.Limitations

There are still some limitations in my program.

1. Users need an internet connection to use Gemini.
2. Users need a valid Gemini API key.
3. Sometimes Gemini cannot answer because the server is busy.
4. Users need to upload a CSV file with the correct format.
5. The chatbot only provides general financial advice and is not a professional financial advisor.

10. AI Assistance

I used ChatGPT to help me during this project.

ChatGPT helped me understand some Python concepts, write example code, and solve errors that happened during development.

For example, I used ChatGPT to understand the Gemini API errors and learn how to fix them.

I also used AI to help organise my README and explain my project.

I ran the code in GitHub Codespaces and checked the results while developing the program.

11. Project Files

ISYS2001_Finance_Assistant.ipynb

This is the main notebook that contains the Python calculations, Gemini chatbot, Gradio interface and testing code.

sample_expenses.csv

This file contains example expenses used to test the program.

README.md

This file explains what my project does and how to use it.

