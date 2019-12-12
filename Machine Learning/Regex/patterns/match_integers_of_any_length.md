---
title: "Match Integers Of Any Length"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match integers of any length in Python."
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
text = '21 scouts and 3 tanks fought against 4,003 protestors.'
```

## Apply regex


```python
# Find any character block that is a integer of any length
re.findall(r'[1-9](?:\d{0,2})(?:,\d{3})*(?:\.\d*[1-9])?|0?\.\d*[1-9]|0', text)
```




    ['21', '3', '4,003']



Explanation from [Justin Morgan](http://stackoverflow.com/users/399649/justin-morgan)

    [1-9](?:\d{0,2}) #A sequence of 1-3 numerals not starting with 0
    (?:,\d{3})*      #Any number of three-digit groups, each preceded by a comma
    (?:\.\d*[1-9])?  #Optionally, a decimal point followed by any number of digits not ending in 0
    |                #OR...
    0?\.\d*[1-9]     #Only the decimal portion, optionally preceded by a 0
    |                #OR...
    0                #Zero.
