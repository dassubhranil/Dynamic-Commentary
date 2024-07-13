# Dynamic-Commentary


## Overview

**Dynamic-Commentary** is a project aimed at exploring the tonal shifts and narrative strategies used by commentators during esports broadcasts. By focusing on popular games like League of Legends, this project seeks to understand how commentators adapt their commentary to the real-time dynamics of the game, creating an engaging and immersive experience for viewers.


## Background

Esports commentary has evolved into a sophisticated craft. Commentators use their voices and storytelling abilities to create an immersive viewing experience. This project delves into how commentators adjust their tone and narrative based on the in-game situation, exploring whether they employ classic storylines like "David and Goliath" to captivate audiences.


## Features

- **Tonal Analysis**: Visualize how commentators' tones change in real-time during a match.
- **Narrative Detection**: Identify common storylines and analogies used by commentators.
- **Interactive Dashboards**: Explore the data through interactive visualizations and dashboards.
- **Case Studies**: Detailed analysis of specific matches and moments.

## Process

1. **Selected a Match for Analysis**:

2. **Used YouTube APIs for Accessing the Video**:

3. **Audio Processing**:
    - Use Pydub to convert the video to machine-friendly audio format and break it into 60-second chunks for effective transcription.

4. **Transcription**:
    - Use ChatGPT API to convert audio segments to text.

5. **Text Cleanup**:
    - Clean up transcribed text to ensure proper sentences and punctuation.

6. **Sentiment Analysis**:
    - Utilize the NLP library `nltk.sentiment.vader` to analyze the sentiment of the commentary and live audience chat.
    - Tokenize and use the nltk tokenize to determine sentiment for each team playing the match.
    - Calculate the sentiment value for each player of the team, and the team itself (including abbreviations used during the commentary), and compound these values over the 60-second audio clips.

7. **Visualization**:
    - Use Python to map out a sentiment plot throughout the game, marking highs, lows, and support swings during gameplay.
