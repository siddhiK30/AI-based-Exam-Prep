
In this task, I developed a Python-based Math Question Processing Pipeline utilizing the Google Gemini API. The objective of this model is to enhance mathematical learning by generating similar questions, providing detailed solutions, and verifying those solutions for accuracy.

Key Features of the Model:

API Configuration:

The pipeline begins by importing necessary libraries and configuring the API key needed for accessing the Gemini model.

Model Initialization:

An instance of the GenerativeModel class is created using the gemini-1.5-flash version, which facilitates content generation based on prompts.

Core Functionalities:

Generate Similar Question:

The function generate_similar_question(original_question_html) rephrases an HTML-formatted math question while changing numeric values, allowing for the creation of diverse practice questions.

Generate Solution:

The function generate_solution_for_question(question_html) solves the generated question step-by-step, providing detailed explanations for each operation, and outputs the final answer in HTML format.

Verify and Correct Solution:

The function verify_and_correct_solution(question_html, solution_html) checks the accuracy of the provided solution. If any discrepancies are identified, it corrects them and presents the accurate solution with comprehensive explanations.

User Interaction:

The math_pipeline() function handles user input, prompting for the original math question in HTML format. It sequentially calls the aforementioned functions to generate a similar question, produce a solution, and verify that solution, displaying results in the console.

Execution:

The entire process is initiated by calling the math_pipeline() function, allowing users to engage with the model and obtain enriched math educational content.

For Math Question Processing Pipeline with Groq API

In this task, I developed a Python-based Math Question Processing Pipeline utilizing the Groq API and the Llama 3 (70 billion parameters) model. The model is designed to assist in generating similar math questions, providing detailed solutions, verifying those solutions, and correcting any inaccuracies.
