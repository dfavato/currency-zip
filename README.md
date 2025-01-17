# currency-zip

![version](https://img.shields.io/badge/version-v0.1.0-white) ![pytest](https://img.shields.io/badge/coverage-100%25-green)

# Purpose

To make banking/invoicing easier. Add currency conversion between multiple income sources and aggregate the total into a single currency.

# Install

Clone the repository and create a Python venv:

```shell
git clone git@github.com:ricardoaugusto/currency-zip.git
cd currency-zip
python3 -m venv .venv
source .venv/bin/activate
```

Check if your .venv is set:

On Windows, change to `python -m venv .venv` and `source .venv\Scripts\activate`.

```shell
$ which python
/Users/ricardoaugusto/dev/currency-zip/.venv/bin/python
```

Finally, install the `requirements.txt`:

```shell
pip install -r requirements.txt
```

# Usage

```shell
python czip.py "100EUR + 250USD + 1000BRL to GBP"
440.19
```

# Test

```shell
 pytest --cov=src tests --cov-report=html:tests/coverage
```

# Contribute