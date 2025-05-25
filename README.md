# MoodMirror
MoodMirror is a smart emotion-based music recommendation system built using deep learning.

When you type a sentence like “I feel gloomy, suggest me sad songs,” it first uses a pre-trained model from Hugging Face called DistilRoBERTa. This model is loaded using the Transformers library and run with TensorFlow, allowing the system to detect your emotion from the text.

The model understands seven emotions — like joy, sadness, anger, and surprise — and predicts the one that best matches your input.

Once your emotion is identified, MoodMirror uses the YouTube Data API to search for songs that match your mood. It uses emotion-specific queries like “soothing emotional piano music” for sadness or “happy upbeat music” for joy.

It then shows you 3 YouTube video links that fit your emotional tone.

Behind the scenes, it uses popular libraries:

TensorFlow to run the model,

Transformers from Hugging Face for natural language understanding,

and Google API Client to fetch music recommendations.
