# Word Frequency Analysis of Literary Texts Using NLP

Completed as part of **Naval Postgraduate School** Cyber Data Management and Analytics.

## Problem

Given a novel hosted on [Project Gutenberg](https://www.gutenberg.org/), extract the full text from HTML, tokenize it, remove stopwords, and produce a word frequency distribution — then generalize the pipeline to analyze any text.

## Pipeline

```
HTTP GET → BeautifulSoup (HTML → text) → RegexpTokenizer → Stopword filter → FreqDist plot
```

1. **Collect** — `requests.get()` fetches raw HTML from Project Gutenberg
2. **Extract** — BeautifulSoup parses HTML to plain text
3. **Tokenize** — `\w+` regex splits text into lowercase words
4. **Filter** — NLTK English stopwords removed
5. **Analyze** — frequency distribution plotted for top-N words

## Texts Analyzed

| Novel | Author |
|-------|--------|
| *Indian Tales* | Rudyard Kipling |
| *War and Peace* | Leo Tolstoy |
| *Ulysses* | James Joyce |
| *King James Bible* | — |

## Quickstart

```bash
git clone https://github.com/lonesome-data/NLP-Project.git
cd NLP-Project
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook nlp_word_frequency.ipynb
```

## Project Structure

```
├── nlp_word_frequency.ipynb         # Analysis notebook (modernized)
├── data/
│   └── stopwords.txt                # Custom stopwords reference
├── requirements.txt                 # Python dependencies
└── NLP_original.ipynb               # Original 2018 notebook (archived)
```

## License

MIT — originally adapted from Hugo Bowne-Anderson's DataCamp tutorial.
