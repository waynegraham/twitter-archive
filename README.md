# Archiving Tweets

This is a wrapper for [https://github.com/DocNow/twarc]

## Requirements

- Python (2 or 3)
- A [Twitter API key](https://apps.twitter.com)

## Generating an Archive

See [twarc usage documentation](https://github.com/DocNow/twarc#usage)

```
$ twarc search '#dlfteach' > dlfteach-tweets.jsonl
$ python twarc/utils/wall.py dlfteach-tweets.jsonl > dlfteach-tweets.html
```

## Installation

```
$ pip install twarc
$ twarc configure
```

## Updating

```
$ git pull
$ git submodule update --remote --merge
```
