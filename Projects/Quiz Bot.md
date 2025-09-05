# Quiz Bot 

## Objective
Design an interactive quiz chatbot for Cloud Learners Inc. using Amazon Lex that tests knowledge about Amazon S3 with multiple-choice questions.

## Steps Taken

Created a new Intent named S3Quiz.

Added quiz-start utterances: “Start quiz,” “Quiz me on S3,” “I’m ready for the quiz.”

Configured the first question:

“What does S3 stand for?”

Options: A) Simple Storage Service, B) Secure Server Storage, C) Smart Storage System

Added conditional responses:

If user chooses A → “Correct! S3 stands for Simple Storage Service. Would you like the next question?”

If user chooses B or C → “Incorrect. The correct answer is Simple Storage Service. Would you like the next question?”

Configured second question:

“What is Amazon S3 mainly used for?”

A) Cloud Storage

B) Web Hosting

C) Cloud Computing

Correct Answer: A

Tested the quiz in the Lex console with both correct and incorrect answers.

## Challenges

Struggled with branching logic when capturing user responses (Lex requires careful slot/condition setup).

Solution: Used conditional responses instead of overcomplicating slots.

The flow initially got stuck after wrong answers.

Solution: Added follow-up prompts (“Would you like the next question?”).

## Screenshots
<img width="1920" height="869" alt="Screenshot (866)" src="https://github.com/user-attachments/assets/33c8273a-b41d-484c-ac35-1b30f5ed709b" />
<img width="1920" height="880" alt="Screenshot (867)" src="https://github.com/user-attachments/assets/b8ee367c-202c-4086-8ba6-eddcf0e094e6" />
<img width="1920" height="866" alt="Screenshot (868)" src="https://github.com/user-attachments/assets/82ca9b9b-1123-434a-b0e2-c084c465d2da" />
<img width="1920" height="869" alt="Screenshot (869)" src="https://github.com/user-attachments/assets/5fee9872-4a7a-441d-bdd6-b761044ef172" />
<img width="1920" height="869" alt="Screenshot (870)" src="https://github.com/user-attachments/assets/38b35f5b-5501-4884-92d2-7c591e92f721" />
<img width="1920" height="873" alt="Screenshot (871)" src="https://github.com/user-attachments/assets/8b0886b0-5716-408b-92df-610971d3f761" />
<img width="1920" height="865" alt="Screenshot (872)" src="https://github.com/user-attachments/assets/19f8daef-509a-45a5-8757-5870534b11eb" />
<img width="1920" height="873" alt="Screenshot (861)" src="https://github.com/user-attachments/assets/e470e82c-bd99-4d40-a8c6-df7ff004afec" />
<img width="1920" height="886" alt="Screenshot (862)" src="https://github.com/user-attachments/assets/93396892-ae5f-4430-9298-a93398e71071" />
<img width="1920" height="862" alt="Screenshot (863)" src="https://github.com/user-attachments/assets/638866af-8e05-475b-97f0-ea6872fc0af2" />
<img width="1920" height="873" alt="Screenshot (864)" src="https://github.com/user-attachments/assets/92b3982d-b684-457f-9661-ff0df7553a81" />
<img width="1916" height="856" alt="Screenshot (865)" src="https://github.com/user-attachments/assets/9ef34a02-44b9-48a7-944c-d3340b07b22c" />


## Takeaways

Amazon Lex supports branching quiz logic using conditions.

Good chatbots give feedback and let the user retry or move on.

Presentation is as important as functionality: explain intents, utterances, responses, and flow in simple terms for clients.
