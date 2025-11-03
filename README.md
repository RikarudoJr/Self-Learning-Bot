# How to run the project?
1. Go to www.botpress.com and Sign in
2. create a new project
3. import the .bpz file
4. Done. Try out the chatbot

# What is this chatbot capable of?
The chatbot can improve its answer on its own based on user feedback. 
Based on the feedbacks, the chatbot is capable of judgding whether to:
1. Reuse past answer
2. Re-generate new answers, that follow the past feedbacks

# But how the chatbot make the judgment?
When the chatbot receive a search query from user, it will do find similar questions asked in the past.
The purpose is to retrieve the answers used in the past, along with its feedback

<img width="1288" height="206" alt="image" src="https://github.com/user-attachments/assets/cc92a366-b40d-4936-a269-09fb8330dcab" />
Feedback Table

Here, the feedbacks from user will be weighted based on recency.
For example, the weight will be halved after certain period:
1. feedback given within 1 week ago: 1 pt
2. feedback given 1 month ago: 0.5 pt
3. feedback given more than 1 month ago: 0.25 pt

When the weight of good feedback - bad feedbacks >0, reuse past answer.
otherwise, re-genarete new answer
# Why choose this judgement method? 
We want to ensure that newer feedbacks are prioritized than past feedbacks.
# Limitation of this judgement method?
Experimentation is needed to see if  good feedback - bad feedbacks >0 is a good enough threshold.
For example, it could be  good feedback - bad feedbacks > 0.5 is a better threshold, etc



