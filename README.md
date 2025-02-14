# Jeugdjournaal (Dutch Youth News) Python Library

A simple Python library for fetching and interacting with articles, polls, comments, and reactions from Jeugdjournaal, all **without the need of authentication**. Made by hcr5.

## Installation

You can install the library via pip:

```bash
pip install jeugdjournaal
```

## Example Usage

Here’s a quick example to get started:

```python
import jeugdjournaal

# Read an article
article = jeugdjournaal.read_item(2528544)
print(article.title)
print(article.content)

# Get poll IDs from the article
poll_ids = jeugdjournaal.get_poll_ids(2528544)
print(poll_ids.id_1)
print(poll_ids.id_2)

# Vote in a poll
jeugdjournaal.vote_in_poll(poll_ids.id_1["id"])
```

For more functions and detailed usage, refer to the [full documentation](https://github.com/hcr5/jeugdjournaal-python/blob/main/docs.md).
