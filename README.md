# Jeugdjournaal Python

## Overview
The `jeugdjournaal` library simplifies interaction with the Jeugdjournaal website and API ([](https://jeugdjournaal.nl)). It provides functionalities to retrieve article details, participate in polls, read/post comments, and explore articles.

## Installation
You can install `jeugdjournaal` via pip:

```
pip install jeugdjournaal
```

## Example Usage
```python
import jeugdjournaal as jj

# Example: Retrieve article details
article_id = '2528081'
article_details = jj.read_item(article_id)
print(article_details['title'])
print(article_details['content'])

# Example: Vote in a poll
poll_id = 'Zdf'
vote_response = jj.vote_in_poll(poll_id)
print(vote_response)

# Example: Retrieve comments
comments = jj.get_comments(article_id, limit=10)
print(comments)
```

## Documentation
For more details, refer to the [documentation](https://github.com/hcr5/SomPy/blob/main/docs.md)
