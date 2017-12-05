
# NLP in Python

<p align="center">
<img src="img/live_preview.jpeg" width="550">
</p>


## Description

<p align="center">
<img src="img/fb_live_schematic.png" width="550">
</p>

Follow the Data Science pipeline to plot frequency distributions of words in *Moby Dick*, or other novels.
Novels are scraped from the website [Project Gutenberg](https://www.gutenberg.org/) (large corpus of books) using the Python package `requests` and extracted using `BeautifulSoup`. Analyze a novel using the Natural Language ToolKit (`nltk`).
The process teaches critical aspects of Natural Language Processing (NLP) such as tokenization and stopwords.
Visualize word frequency distributions of any novel from Project Gutenberg.
The NLP skills developed, however, are applicable to much of what Data Scientists encounter as the vast proportion of the world's data is unstructured data and includes a great deal of text.

## Prerequisites

Mininal. Familiarization with...

* programming fundamentals and the basics of the Python programming language (e.g., variables, for loops);
* a bit about Jupyter Notebooks;
* your way around the terminal/shell.

Install the [Anaconda distribution](https://www.anaconda.com/download/) of Python 3 (see below).


## Getting set up computationally

### 1. Clone the repository

You can do so by executing the following in your terminal:

```
git clone https://github.com/lonesome-data/CY3650-Project
```

Alternatively, you can download the zip file of the repository at the top of the main page of the repository. If you prefer not to use git or don't have experience with it, this a good option.

### 2. Download Anaconda (if you haven't already)

If you do not already have the [Anaconda distribution](https://www.anaconda.com/download/) of Python 3, go get it (n.b., you can also do this w/out Anaconda using `pip` to install the required packages, however Anaconda is great for Data Science and you are encouraged to use it).

### 3. Create your conda environment for this session

Navigate to the relevant directory `CY3650-Project` and install required packages in a new conda environment:

```
conda env create -f environment.yml
```

This will create a new environment called CY3650_nlp. To activate the environment on OSX/Linux, execute

```
source activate CY3650_nlp
```
On Windows, execute

```
activate CY3650_nlp
```


### 4. Open your Jupyter notebook

In the terminal, execute `jupyter notebook`.

Then open the notebook `CY3650_NLP.ipynb` and we're ready to get coding. Enjoy.


### Code
The code in this repository is released under the [MIT license](LICENSE). Read more at the [Open Source Initiative](https://opensource.org/licenses/MIT). All text remains the Intellectual Property of DataCamp. If you wish to reuse, adapt or remix, get in touch with me at hugo at datacamp com to request permission.
