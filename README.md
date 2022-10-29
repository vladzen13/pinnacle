## About this fork

Original repo seems dead, no commits or merges for years.

Cleaned up requirements, fixed tests and bumped docker python image version to nice and fast 3.11

Fixed issue with installation failure in environment without requests package (caused by importing requests while __version__ reading in setup.py file)


# Install this fork:

```
$ pipenv --python 3.11

$ pipenv install https://github.com/vladzen13/pinnacle/archive/master.zip
```

## Original repo README

# pinnacle
Python Wrapper for Pinnacle Sports API

[Pinnacle Documentation](https://www.pinnacle.com/en/api/manual)

# Installation

```
$ pip install pinnacle
```

# Usage

```python
>>> from pinnacle.apiclient import APIClient
>>> api = APIClient('username', 'password')
>>> sport_ids = api.reference_data.get_sports()
>>> tennis_events = api.market_data.get_fixtures(33)
```
