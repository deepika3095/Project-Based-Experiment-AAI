<H3>NAME: PREETHI A K</H3>
<H3>REGISTER NO: 212223230156</H3>
<H1 Align="center">Project Based Experiment<H1>

## Objective:
Perform sentiment analysis using your Facebook data and filter the data that has only neutral feedback for the code
## Program:
  
  ```py
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer

nltk.download('vader_lexicon')

sia = SentimentIntensityAnalyzer()

facebook_data = [
    "I love the new feature! It's amazing.",
    "The service was terrible. I'm very disappointed.",
    "Great job on the update!",
    "The product quality is poor. I won't be buying again.",
    "It is okay, nothing special.",
    "The app works as expected.",
    "I think it's fine overall.",
    "Nothing much to say about this update.",
    "The experience was average.",
    "Not good, not bad, just okay.",
    "I absolutely love how this app looks!",
    "Customer support was not helpful at all.",
    "It's working normally without issues.",
    "I feel the design is acceptable.",
    "Could be better but it's fine."
]

neutral_feedback = []

for message in facebook_data:
    sentiment_score = sia.polarity_scores(message)['compound']
    
    if -0.05 < sentiment_score < 0.05:  
        neutral_feedback.append(message)

print("Neutral Feedback:")
for feedback in neutral_feedback:
    print(feedback)

 ```

## OUTPUT:
<img width="813" height="144" alt="image" src="https://github.com/user-attachments/assets/1a3c682c-d89f-48c6-8a40-1772a9ab787b" />


<H3>RESULT:</H3>
 A sentiment analysis project using Facebook data provides valuable learning experiences in data handling, text processing, sentiment analysis, and ethical considerations, while also honing communication, problem-solving, and project management skills.
