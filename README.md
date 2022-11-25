#clone your project


Create virtual environment

## python3 -m venv venv
## venv\Scripts\activate

install pytorch and dependencies

## you also need nltk
## pip install nltk

If you get an error during the first run, you also need to install nltk.tokenize.punkt: Run this once in your terminal:

## import nltk
## nltk.download('punkt')

first run the *******python train.py**** file  This will dump data.pth file. And then run

## python chat.py


***************************JSON FILE IS VERY IMPORTANT**************************************

Have a look at intents.json. You can customize it according to your own use case. Just define a new tag, possible patterns, and possible responses for the chat bot. You have to re-run the training whenever this file is modified.

{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
