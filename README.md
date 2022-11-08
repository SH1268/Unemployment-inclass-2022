# Unemployment-inclass-2022

## Setup

Create and activate a virtual environment:

conda create -n unemployment-env python=3.8

conda activate unemployment-env



Install package dependencies:

pip install -r requirements.txt


## Configuration

[Obtain an API Key] https://www.alphavantage.co/support/#api-key. from ALPHAVANTAGE

Then create a local ".env" file and provide the key like this:

 
ALPHAVANTAGE_API_KEY="_________"


## Usage

Run the example script:

python app/my_file.py

'''

Run the unemployment report:

python app/unemployment.py

Run stocks report:

```
python app/stocks.py
```

### or pass env var from command line:
ALPHAVANTAGE_API_KEY="_____" python app/unemployment.py


