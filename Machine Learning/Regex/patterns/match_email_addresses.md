---
title: "Match Email Addresses"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match email addresses in Python."
type: technical_note
draft: false
---
## Preliminaries


```python
# Load regex package
import re
```

## Create some text


```python
# Create a variable containing a text string
text =  'My email is chris@hotmail.com, thanks! No, I am at bob@data.ninja.'
```

## Apply regex


```python
# Find all email addresses
re.findall(r'[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9]+', text)

# Explanation:
# This regex has three parts
# [a-zA-Z0-9_.+-]+ Matches a word (the username) of any length
# @[a-zA-Z0-9-]+  Matches a word (the domain name) of any length
# \.[a-zA-Z0-9-.]+ Matches a word (the TLD) of any length
```




    ['chris@hotmail.com', 'bob@data.ninja']


