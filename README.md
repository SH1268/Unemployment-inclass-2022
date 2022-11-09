# Unemployment-inclass-2022

## Setup

Create and activate a virtual environment:

conda create -n unemployment-env python=3.8

conda activate unemployment-env



Install package dependencies:

```sh 
pip install -r requirements.txt
```

## Configuration

[Obtain an API Key] https://www.alphavantage.co/support/#api-key. from ALPHAVANTAGE

Then create a local ".env" file and provide the key like this:

 
ALPHAVANTAGE_API_KEY="_________"


## Usage

Run the example script:

```sh 
python -m app.my_file
``` 

Run the unemployment report:

```sh 
python -m app.unemployment
```

Run stocks report:

```sh
python -m app.stocks
```

### or pass env var from command line:
```sh 
ALPHAVANTAGE_API_KEY="_____" python app/unemployment.py
```

## Testing

Run tests:

```sh 
pytest
```