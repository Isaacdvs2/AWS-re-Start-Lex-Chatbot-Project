# AWS-re-Start-Lex-Chatbot-Project

## Authors
---
<details>
<summary>View Contributors/Authors</summary>
>aka Group 3
- Masekela Isaac Maake
- Gugulethu Oliphant
- Mr. Raven Phadagi
- Tumelo Moyi
</details>

---

### Introduction
The aim of this project is to design a chatbot using AWS Lex. 

---

### 1. Business Context & Requirements
#### Business Context
Cloud Learners Inc. is an educational technology startup that provides online training and certification preparation for cloud computing, with a focus on Amazon Web Services (AWS). To improve learner engagement and reinforce knowledge after lessons, the company wants to introduce an interactive chatbot that can quiz learners on AWS concepts.

Rather than presenting learners with a traditional multiple-choice assessment, the company aims to provide a conversational quiz experience using Amazon Lex. 

The initial implementation will focus on AWS CodeCommit and **[Tumelo Updates]**, with the possibility of expanding the chatbot to cover additional AWS services such as Amazon EC2, AWS Lambda, Amazon VPC, and AWS IAM in the future.

#### Business Requirements
The chatbot should:

- Welcome learners and introduce the quiz.
- Explain the quiz rules before starting.
- Ask a series of questions about Amazon CodeCommit and **[Tumelo's Update]**.
- Accept user responses through natural language.
- Determine whether each answer is correct or incorrect.
- Provide immediate feedback after every question.
- ***Maintain the learner's score throughout the quiz.***
- ***Display the final score at the end of the quiz.***
- Ask whether the learner would like to retake the quiz.
- End the conversation politely if the learner chooses not to continue.

#### Functional Requirements
Functional requirements describe What the system must do.
The solution must:

- Be developed using Amazon Lex.
- Support conversational interactions through intents and sample utterances.
- Guide users through the quiz using prompts and responses.
- Validate user input where necessary.
- Keep track of quiz progress.
- Calculate and display the learner's final score.
- Provide a simple and user-friendly conversational experience.

### Non-Functional Requirements

The chatbot should be:

- Easy to use for beginner cloud learners.
- Responsive, with minimal delays between questions.
- Accurate in evaluating user responses.
- Easy to maintain and extend with additional AWS service quizzes.
- ***Available through supported Amazon Lex deployment channels.***

### 2. Amazon Lex Overview
#### What is Amazon Lex?

Amazon Lex is a fully managed AWS service for building conversational chatbots that interact with users through text or voice. It enables developers to create chatbots capable of understanding user input, managing conversations, and providing interactive responses.

Originally, Amazon Lex was designed around Natural Language Understanding (NLU), where developers manually define the chatbot's **intents**, sample **utterances**, **slots**, and **conversation flow**(logic).

Amazon Lex has introduced support for Large Language Models (LLMs) through integration with services such as Amazon Bedrock, allowing developers to build more intelligent and flexible conversational experiences.

For this project, the traditional Amazon Lex approach was selected

### 3. Solution Overview
The proposed solution is an interactive rule-based quiz chatbot developed using Amazon Lex. This solution follows a predefined conversational flow. The chatbot uses intents, sample utterances, slots, and preconfigured responses to guide learners through the quiz and provide immediate feedback based on their answers. The flow diagram of the solution is shown in the image below.
<a href="./resources/AWSLexFlow.png">
  <img src="./resources/AWSLexFlow.png" 
       alt="AmazonLexFlow" 
       style="width: 100%; max-width: 900px; height: auto;">
</a>


When a learner starts the chatbot, they are welcomed and introduced to the quiz. The chatbot then asks a series of Amazon S3 questions, one at a time. After each response, the chatbot evaluates the answer against predefined correct answers, informs the learner whether their answer is correct or incorrect, and updates their score. Once all questions have been completed, the chatbot displays the learner's final score and offers the option to retake the quiz or end the conversation.






### 4. Lessons Learnt

### 5. Recommendation