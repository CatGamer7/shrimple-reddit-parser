# About
Shrimple Reddit Parser - a basic CLI utility for parsing reddit communities with PRAW. It is as [shrimple](https://ih1.redbubble.net/image.5476092038.1933/bg,f8f8f8-flat,750x,075,f-pad,750x1000,f8f8f8.jpg) as that, really.

# Project structure
1. [main.py](/main.py) - CLI definition;
2. [/parser/data_model](/parser/data_model/) - Data formats;
3. [/parser/parser.py](/parser/parser.py) - Parser logic.

# Overview
This parser aims to extract to submissions and their comments from the specific subreddit. Submissions are searched for by flairs and keywords.

There are several parsing modes:
1. Extract submissions with passed flairs. Will ignore all submissions with no flairs (will only extract newer submissions).
2. Extract submissions with passed keywords and no passed flairs. Will ignore newer submissions.
3. Extract submissions with passed keywords regardless of flairs. 

Try the following command to get descriptions of all the CLI arguments
```python3 main.py -h```

To use this shrimple parser you have to register for Reddit API like [here](https://github.com/reddit-archive/reddit/wiki/OAuth2-Quick-Start-Example#first-steps).
