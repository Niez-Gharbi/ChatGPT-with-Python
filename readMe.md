# ChatGPT APIs in Python

## Setup

### Get an API key

Log into [OpenAI website](https://openai.com/) and, if you are not on the free tier, add a credit card. 
After that go to the profile section (top right) and click on `View API keys`.

Then click on `Create new secret key` and store your key.

Eithger add your key to your environment variables `export OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>`, or in code using `openai.api_key = <API-KEY>`.
 

### Install pip package

Now, install the [`openai` pip package](https://github.com/openai/openai-python) 

```
pip install --upgrade openai
```

## Make a simple request

The official doc is [here](https://platform.openai.com/docs/guides/chat?utm_medium=email&_hsmi=248334739&utm_content=248334739&utm_source=hs_email). 

To make a simple request, you can run the main script and ChatGPT will respond to your question.

```
python main.py
```

`messages` is a list of dictionaries with key `role` and `content`. `role can be `system`, use it to set the bot behaviour, `user` is the user interacting with the bot (ourself) and `assistant` is the chatbot. Inside `content` we place our text.

## Creating a chat cli

We can go one step further by creating a little interactive chat we can run in the terminal

```python
python cli.py
```

## Conclusion

This project is inspired by [how-to-use-chatgpt-with-python](https://github.com/FrancescoSaverioZuppichini/how-to-use-chatgpt-with-python)
