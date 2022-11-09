# Unemployment-inclass-2022

## Configuration


[Obtain an API Key](https://www.alphavantage.co/support/#api-key) from AlphaVantage.
[Obtain an API Key](https://www.alphavantage.co/support/#api-key) from AlphaVantage (i.e. `ALPHAVANTAGE_API_KEY`).

Then create a local ".env" file and provide the key like this:
Also sign up for the [SendGrid Service](https://sendgrid.com/), verify your single sender address (i.e. `SENDER_EMAIL_ADDRESS`), and obtain an API Key (i.e. `SENDGRID_API_KEY`). See these [setup notes](https://github.com/prof-rossetti/intro-to-python/blob/main/notes/python/packages/sendgrid.md#setup) for more details.

Then create a local ".env" file and provide the keys like this:

```sh
# this is the ".env" file...
ALPHAVANTAGE_API_KEY="_________"
SENDER_EMAIL_ADDRESS="you@example.com"
SENDGRID_API_KEY="__________"
```

Run the unemployment report:

```sh
#python app/unemployment.py
# or pass env var from command line:
#ALPHAVANTAGE_API_KEY="______" python app/unemployment.py
python -m app.unemployment
```

Run stocks report:

```sh
#python app/stocks.py
python -m app.stocks
```


### Email Sending

Run the email service to send an example email and see if everything is working:

```sh
python -m app.email_service
```

Send the unemployment report via email:

```sh
python -m app.unemployment_email
```

Send the stocks report via email:

```sh
python -m app.stocks_email
# or in production mode:
APP_ENV="production" DEFAULT_SYMBOL="GOOGL" python -m app.stocks_email
```

## Testing

Run tests:
```sh
pytest
```