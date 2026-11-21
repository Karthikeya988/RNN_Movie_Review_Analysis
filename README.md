# Movie Review Sentiment Analysis

A small notebook project that classifies IMDb movie reviews as positive or negative with a PyTorch recurrent neural network.

## Features

- Cleans review text and removes stop words
- Stems words with NLTK
- Converts text to TF-IDF features
- Trains and evaluates a binary sentiment classifier

## Tech Stack

Python, pandas, NLTK, scikit-learn, PyTorch, and Jupyter.

## Data

The notebook expects `data/IMDB Dataset.csv` with `review` and `sentiment` columns. The local dataset is excluded from Git because this project's copy is 66 MB, its source and redistribution license are not documented, and a scan found email-shaped text in the reviews. Obtain a copy from a source whose terms permit your intended use before adding or redistributing it. Do not commit the supplied local data file without checking its provenance, license, and contents.

## Installation

Use Python 3.10 or newer, then install the dependencies:

```bash
python -m venv .venv
```

Activate the environment (`.venv\Scripts\activate` on Windows, or `source .venv/bin/activate` on macOS/Linux), then run:

```bash
python -m pip install -r requirements.txt
```

## Usage

Place the permitted dataset at `data/IMDB Dataset.csv`, open `RNN_MovieReviews_prac.ipynb` in Jupyter, and run the cells in order. NLTK downloads its tokenizer and stop-word data on the first run, which requires network access.

## Results

The notebook prints training loss and held-out accuracy when run. No verified run or reproducible metric is included in this repository, so no accuracy value is reported here.