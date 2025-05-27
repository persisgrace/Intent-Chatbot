# Intent-Chatbot

This project is a simple intent-based chatbot built using Python, Natural Language Processing (NLP), and Machine Learning. The chatbot classifies user messages into predefined intents and responds accordingly.

## Features

- **Machine Learning Based:** Uses logistic regression and TF-IDF vectorization for intent classification.
- **NLP:** Utilizes NLTK for text preprocessing.
- **Web Interface:** Built with Streamlit for an interactive chat experience.
- **Conversation History:** Logs all chats to a CSV file.
- **Easy to Extend:** Add new intents and responses by editing the JSON file.

## Setup Instructions

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/intent_chatbot.git
    cd intent_chatbot
    ```

2. **Install dependencies:**
    ```bash
    pip install streamlit scikit-learn nltk joblib
    ```

3. **Download NLTK data:**
    ```python
    import nltk
    nltk.download('punkt')
    ```

4. **Run the chatbot:**
    ```bash
    streamlit run final_app.py
    ```

## Project Structure

```
intent_chatbot/
├── final_app.py                  # Main Streamlit app
├── intents_dataset_aicte.json    # Intents and responses
├── chat_log.csv                  # Conversation history (auto-generated)
└── nltk_data/                    # NLTK data (auto-downloaded)
```

## How It Works

- The chatbot loads intents and example phrases from a JSON file.
- It trains (or loads) a logistic regression model to classify user input.
- When a user sends a message, it predicts the intent and returns an appropriate response.
- All conversations are saved in a CSV file for later review.

## Customization

- **To add new intents or responses:** Edit `intents_dataset_aicte.json` and retrain the model.

## License

This project is open-source and available under the MIT License.

---

**Enjoy chatting!**
