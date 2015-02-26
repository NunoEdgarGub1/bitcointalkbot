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

## Deployment

Push the app to Heroku:

```bash
$ heroku create my-application-name
$ git push heroku master
```

### Configuration

The following config vars are required:
 - `KEYWORDS`: a comma separated list of keywords to listen on
 - `SLACK_API_TOKEN`: Slack authentication token
 - `SLACK_USERNAME`: Username for bot on Slack
 - `SLACK_CHANNEL`: Channel to post updates on Slack
