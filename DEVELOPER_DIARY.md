# Developer Diary – Smart Personal Budget Assistant

**Development time:** Approximately 5 hours

## Project Development

I completed most of this project in around 5 hours. I started by planning a personal budget assistant for university students. Then I created Python functions to calculate expenses, remaining balance and spending percentage.

After that, I used pandas to read a CSV file and calculate expenses for different categories.

## Gemini API and Gradio

The most difficult part was connecting Gemini API. At first, I had problems with my API key and some Python errors. I also received a 503 error because Gemini was too busy.

I used `getpass()` to enter my API key and added error handling to manage the Gemini problem.

Next, I used Gradio to create a simple interface where users can enter their income, upload a CSV file and ask financial questions.

## Testing and Debugging

I added `assert` tests to check my calculations. I also faced a `NameError` because I did not run my earlier function cell.

I learned how to check errors and run notebook cells in the correct order.

## AI Assistance

I used ChatGPT during this project to understand the assessment requirements, get example code, fix Python errors and help write my documentation.

Some parts of the code were suggested by ChatGPT, especially the Gemini and Gradio sections. I copied and adapted the code and tested it in GitHub Codespaces.

## Reflection

This project helped me learn more about Python, pandas, Gemini API and Gradio. I still need more practice with programming, especially understanding errors and connecting different parts of the code.