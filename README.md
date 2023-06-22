# Lib2 - Python Lib

<!-- [![codecov](https://codecov.io/gh/author_name/project_urlname/branch/main/graph/badge.svg?token=project_urlname_token_here)](https://codecov.io/gh/author_name/project_urlname)
[![CI](https://github.com/author_name/project_urlname/actions/workflows/main.yml/badge.svg)](https://github.com/author_name/project_urlname/actions/workflows/main.yml) -->

This python package contains some useful common methods for data preprocessing on the restaurant sentiment analysis project.

## Install it from PyPI

```bash
pip install lib2 # latest
pip install lib2=1.0.0 # specific version
```

## Usage
The library's usage is demonstrated below

```py
from lib2.version_util import VersionUtil
from lib2.preprocessing import prepare_stopwords, preprocess_data

# Get the version of lib2 being used.
VersionUtil.get_version() 

# Uses the PorterStemmer & english stopwords from nltk
stopwords, stemmer = prepare_stopwords()

preprocess_text = preprocess_data(raw_text, stemmer, stopwords)
```
