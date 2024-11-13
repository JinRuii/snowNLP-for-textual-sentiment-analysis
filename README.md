# 📊 Sentiment Analysis of Chinese Comments

This project leverages **SnowNLP**, a powerful library designed for Chinese natural language processing (NLP). SnowNLP allows us to analyze Chinese text data for various applications, including sentiment analysis, keyword extraction, and more. Here, we use SnowNLP to perform sentiment analysis, calculating the emotional tone of user comments and feedback.

For more details on SnowNLP’s full capabilities, visit the [original SnowNLP GitHub repository](https://github.com/isnowfy/snownlp).

### 🏙️ Application of Sentiment Analysis in Urban Planning

In urban planning, understanding public sentiment can offer invaluable insights into community needs, preferences, and perceptions about public spaces and services. By analyzing social media comments, public surveys, or feedback from residents, urban planners can:

- **Assess public satisfaction** with urban amenities, like parks, transport, and public facilities.
- **Identify potential areas of improvement** by analyzing negative sentiment patterns.
- **Capture regional differences** in public opinion, helping to guide localized planning efforts.
- **Understand psychological responses** to different spaces, which can be crucial for designing inclusive and accessible environments for diverse age groups and needs.

This project provides a foundation for sentiment analysis in urban planning, helping planners gauge public sentiment and integrate this understanding into more responsive urban designs.

## 📁 Project Structure

- **`📂 data/`**: Directory to store CSV files (input and output).
  - **`📄 sample.csv`**: Input file with comments for sentiment analysis.
  - **`📄 Comments_with_sentiment.csv`**: Output file with calculated sentiment scores.

- **`📄 sentiment_analysis.py`**: Main script that processes the comments, calculates sentiment scores, and saves the output.

## ⚙️ Requirements

- **Python 3.6+**
- **SnowNLP**: A Python library for Chinese Natural Language Processing.
- **pandas**: For data handling.
- **matplotlib**: For plotting sentiment scores.
- **numpy**: For numerical operations.

Install the necessary packages using:

```bash
pip install snownlp pandas matplotlib numpy


## 📁 Explanation of the Script
The script loads comments from `sample.csv` and uses `SnowNLP` to calculate a sentiment score for each comment (ranging from 0 to 1).
Optionally, the score can be adjusted to a range of [-0.5, 0.5], centering it around zero to make the data more interpretable. This adjustment is optional.
A plot displays the sentiment score distribution across comments, showing how sentiments vary within the dataset.
Finally, the processed data, including the sentiment scores, is saved as `Comments_with_sentiment.csv`.
