# What is this project about?
This is a chatbot that can improve answer on its own based on user feedback. 
Based on the feedbacks, the chatbot is capable of judgding whether to:
1. Reuse past answer
2. Re-generate past answer

# How the chatbot make the judgment?
Here, the feedbacks from user will be calculated based on recency.
Each time it is past a week, the point will be halved
For example:
1. If it was within 1 week: 1 pt
2. If it was within 1-2 weeks: 0.5 pt
3. If it was within 2-3 weeks: 0.25 pt

# What this solution is good for: 
# What this solution lacks

