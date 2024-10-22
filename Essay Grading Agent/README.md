# Essay Grading Agent

This project demonstrates an **Essay Grading Agent** created using the **LangGraph framework**. The agent is capable of grading essays by analyzing the structure, grammar, and content of essays, and it provides feedback based on predefined criteria. The agent integrates natural language understanding and graph-based decision-making to produce robust and accurate results.

## Features

- **Automated Essay Grading**: Grades essays based on content, structure, language, and grammar.
- **Feedback Generation**: Provides feedback on areas where the essay can be improved.
- **Customizable Criteria**: Easily adjustable grading rubric to suit different grading standards or requirements.
- **Multi-Step Reasoning**: Breaks down the grading process into multiple steps, ensuring thorough evaluation.

## How It Works

The Essay Grading Agent leverages **LangGraph**, a framework designed to combine language models with graph-based reasoning. Here's a high-level overview of how the agent works:

### 1. **Input Parsing**
   The agent receives an essay and topic as input in the form of text. The essay is then tokenized and parsed for structural elements like introduction, body, and conclusion.

### 2. **Grading Criteria**
   The agent uses a predefined set of criteria to evaluate the essay. This could include:
   - **Content Relevance**: Does the essay address the prompt or question?
   - **Grammar and Syntax**: Does the essay use correct grammar and sentence structure?
   - **Vocabulary and Fluency**: Is the vocabulary appropriate and varied?

### 3. **Graph-Based Evaluation**
   Using the LangGraph framework, the agent follows a graph-based workflow:
   - **Nodes**: Each node in the graph represents a specific aspect of the grading process (e.g., grammar check, structure analysis).
   - **Edges**: Edges define the flow between nodes, ensuring that each part of the essay is evaluated in sequence.
   - **Decision Making**: The agent makes decisions based on the evaluation of each criterion, assigning scores and generating feedback accordingly.

### 4. **Scoring and Feedback**
   Once the essay is graded across all criteria, the agent calculates the final score and generates detailed feedback on how the essay can be improved. The feedback is designed to be constructive, giving the student clear guidance on what they can do better.

4. **Customizing the Grading Criteria**:
   You can modify the grading criteria by adjusting the nodes in the LangGraph structure. Each node corresponds to a specific grading task, and you can easily change the weights or add new nodes to fit your needs.

5. **View the Results**:
   The notebook will output the final grade along with feedback for the essay. You can tweak the output formatting or extend the analysis to include more detailed reports if needed.


## Customization

- **Adjust the Rubric**: The grading criteria can be adjusted in the graph by modifying the scoring nodes. You can update the scoring range, change the feedback text, or add new evaluation criteria.
- **Support for Multiple Formats**: While this agent currently handles text-based essays, it can be extended to handle other formats like PDFs or DOCX files.
