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
<img width="1288" height="206" alt="image" src="https://github.com/user-attachments/assets/cc92a366-b40d-4936-a269-09fb8330dcab" />

Here, the feedbacks from user will be weighted based on recency.
Each time it is past a week, the point will be halved
For example:
1. If it was within 1 week: 1 pt
2. If it was within 1-2 weeks: 0.5 pt
3. If it was within 2-3 weeks: 0.25 pt

# Why choose this judgement method? 
We want to ensure that newer feedbacks are prioritized than past feedbacks.
# Limitation of this judgement method?



