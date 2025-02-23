# TestAgentBot

Agents in the Agentic Quiz System
Quiz Master Agent (Primary Controller)
Role: Oversees the entire quiz flow, determines difficulty, and manages user interaction.
Actions:
Tracks user progress and selects appropriate questions.
Decides whether to generate, modify, or repeat a question.
Delegates tasks to other agents as needed.

Question Generation Agent (LLM-powered Generator)
Role: Uses the Gemini API to create questions dynamically.
Actions:
Generates new questions based on topic and difficulty.
Rewrites questions for clarity if flagged by other agents.
Expands on concepts when required.

Knowledge Verification Agent (Fact-Checker)
Role: Ensures that generated questions and answers are correct and well-formed.
Actions:
Cross-checks questions against a knowledge base or external API (Wikipedia, WolframAlpha, etc.).
Flags incorrect or ambiguous questions and asks for refinement.
Verifies correctness of AI-generated answers before presenting them.

Adaptive Learning Agent (Personalization Manager)
Role: Adjusts question difficulty and tracks user strengths/weaknesses.
Actions:
Stores user responses and adjusts difficulty dynamically.
Suggests related questions if a user struggles with a topic.
Keeps a memory of past performance to personalize future quizzes.

Explanation & Feedback Agent (Answer Evaluator)
Role: Provides explanations for correct/incorrect answers and enhances learning.
Actions:
Offers detailed explanations for each answer.
Suggests external resources or hints for incorrect answers.
Can engage in a conversational mode to explain concepts interactively.
Engagement & Interaction Agent (Chatbot/Voice Interface)

Role: Enhances user experience by making the quiz interactive and engaging.
Actions:
Uses voice or chat interface to interact naturally.
Adjusts responses based on user engagement level.
Encourages users with motivational messages.

How These Agents Work Together
User starts the quiz → 
The Quiz Master Agent reviews past user data and selects the first question.
The Question Generation Agent creates a new question or retrieves a stored one.
The Knowledge Verification Agent checks if the question is valid.
The Adaptive Learning Agent adjusts difficulty based on the user’s past performance.
The user submits an answer.
The Explanation & Feedback Agent evaluates the response and provides explanations.
The Engagement & Interaction Agent keeps the user motivated.
The cycle repeats, improving the experience with each question.
