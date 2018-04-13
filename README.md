# Archiving Tweets

This is instructions for generating a web 'wall' using [twarc](https://github.com/DocNow/twarc) for twitter conversations.

## Requirements

- Python (2 or 3)
- [pip](https://docs.python.org/3/installing/)
  - **macOS** `brew install brew-pip`
- A [Twitter API key](https://apps.twitter.com)

## Generating an Archive

See [twarc usage documentation](https://github.com/DocNow/twarc#usage)

```
$ twarc search '#dlfteach' > dlfteach-tweets.jsonl
$ python twarc/utils/wall.py dlfteach-tweets.jsonl > dlfteach-tweets.html
```

## Installation

```
$ git clone --recursive https://github.com/waynegraham/twitter-archive.git
$ pip install twarc
$ twarc configure
```

## Updating

```
$ git pull
$ git submodule update --remote --merge
```

## @#$!@ I forgot to initialize the submodule

```
$ cd path/to/twitter-archive
$ git submodule init
$ git submodule update
```
