🧠 AI Prompt Generator – Workflow Documentation
📘 Overview

The AI Prompt Generator is an automated workflow designed to collect user input, generate relevant and context-based questions, and ultimately create a structured AI prompt ready for use in generative AI systems.
It combines user interaction with intelligent question generation and refinement using a chat model (Google Gemini Chat Model).

⚙️ Workflow Structure
1️⃣ Initiate and Get the Basic Questions

Trigger: On form submission

Purpose: Collect initial input or basic questions from the user.

Components:

On form submission: Starts the workflow when the user submits the initial form.

BaseQuestions: Defines or retrieves basic questions from the “Next Form Page.”

2️⃣ Generate Relevant Questions

Purpose: Generate more detailed or related questions using an AI model.

Components:

RelatedQuestion AI: Uses Google Gemini Chat Model to create follow-up questions.

Structured Output Parser: Ensures the generated questions are properly formatted for use in the next step.

3️⃣ Ask Questions to the User

Purpose: Interactively ask the user the generated questions and collect responses.

Components:

SplitQuestions: Divides questions for sequential asking.

LoopQuestions: Iterates over each question.

RelevantQuestions Form Page: Presents each question to the user.

MergeUserIntent: Combines user responses and relevant question data for prompt generation.

4️⃣ Prompt Generator System

Purpose: Generate a refined AI prompt based on collected user responses.

Components:

PromptGenerator AI: Generates the final AI prompt using Google Gemini Chat Model.

Auto-Fixing Output Parser: Validates and fixes any formatting issues in the output.

Structured Output Parser 1: Ensures the output is structured and ready for display or use.

5️⃣ Sending the Prompt to User

Purpose: Deliver the finalized prompt to the user.

Components:

SendingPrompt: Displays or sends the final prompt output through the “Form Ending” step.

🧩 Data Flow Summary

User Input → Initial form submission.

Basic Questions → AI generates additional relevant questions.

User Interaction → User answers generated questions.

Prompt Generation → AI model creates a refined prompt.

Prompt Delivery → Final prompt is sent to the user.

🤖 AI Model Used

Model: Google Gemini Chat Model

Functions:

Generate related questions

Create the final prompt

Auto-fix and structure the AI output

🧱 Key Features

Dynamic question generation based on user input

Structured output parsing for consistent formatting

Auto-correction of malformed responses

Modular workflow design (easy to modify or expand)

📤 Output Example

Final Output: A refined AI prompt ready to use in any AI or automation context.
