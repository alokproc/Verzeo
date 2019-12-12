---
title: "Match US Phone Numbers"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match US phone numbers in Python."
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
text = 'My phone number is 415-333-3922. His phone number is 4239389283'
```

## Apply regex


```python
# Find any text that fits the regex
re.findall(r'\(?([2-9][0-8][0-9])\)?[-.●]?([2-9][0-9]{2})[-.●]?([0-9]{4})', text)
```




    [('415', '333', '3922'), ('423', '938', '9283')]


