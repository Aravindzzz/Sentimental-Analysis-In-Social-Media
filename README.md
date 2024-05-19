# Twitter Sentiment Analysis App 

This is a Streamlit web application that allows users to register, log in, and analyze the sentiment of their tweets. The app uses a pre-trained sentiment analysis model to classify tweets as Positive, Negative, Neutral, or Irrelevant. Users under the age of 18 are restricted to posting only positive tweets. The app also displays a sentiment distribution pie chart for the logged-in user's tweets. 

## Project Structure

- `app.py`: Main application code.
- `requirements.txt`: List of required Python packages.
- `Twitter_sentiment.pkl`: Pre-trained sentiment analysis model.
-  [Open ML Model in Google Colab](https://colab.research.google.com/drive/1x66LutDR-55EQyz4MQfKYlH06ZaeFaHA?usp=sharing)
-  train the model in jupyter or colob using the previous link and a .pkl file will be created which is your pretrained ML model.

## Features

- **User Registration and Login**: Users can register with an email and password, and log in to access the app.
- **Sentiment Analysis**: Users can input tweets, and the app will predict the sentiment (Positive, Negative, Neutral) and relevance (Relevant, Irrelevant).
- **Tweet Posting**: Users can post tweets. Users under 18 can only post positive tweets, and negative irrelevant tweets cannot be posted.
- **Tweet History**: Users can see their previously posted tweets after logging back in.
- **Sentiment Distribution**: A pie chart showing the distribution of tweet sentiments for the logged-in user.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/twitter-sentiment-analysis-app.git
    cd twitter-sentiment-analysis-app
    ```

2. **Install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Download the pre-trained models**:
    - Place `Twitter_sentiment.pkl` in the project directory.

## Usage

1. **Run the Streamlit app**:
    ```bash
    streamlit run app.py
    ```

2. **Open the app in your browser**:
    The app will typically be available at `http://localhost:8501`.

## How It Works

1. **Registration and Login**: Users can register with their email, password, and age. The registration information is stored in the session state.
2. **Sentiment Analysis**: Users can input a tweet, and the app uses a pre-trained model to predict the sentiment and relevance of the tweet.
3. **Posting Tweets**: Based on the sentiment and user's age, the app determines if the tweet can be posted. The tweets are stored in the session state and displayed in the app.
4. **Sentiment Distribution**: A pie chart shows the distribution of the sentiments of the user's posted tweets.

## Future Improvements

- Add a database to persist user data and tweets across sessions.
- Improve the relevance prediction model.
- Enhance the user interface for a better user experience.





