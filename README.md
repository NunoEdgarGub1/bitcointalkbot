# BitcoinTalk Bot

For monitoring keywords on Bitcointalk, and posting them to Slack.

Forked with the following improvements:
 - Straightforward Heroku deployment
 - Code cleanup and standardization

## Dev

Setup the virtual environment, and run:

```bash
$ mkvirtualenv bitcointalkbot -p `which python3`
$ pip install -r requirements.txt
$ python crawler.py
```
