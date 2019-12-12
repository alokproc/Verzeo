---
title: "Match Any Of A List Of Characters"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match any of a list of characters in Python."
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
text = 'The quick brown fox jumped over the lazy brown bear.'
```

## Apply regex


```python
# Find all instances of any vowel
re.findall(r'[aeiou]', text)
```




    ['e', 'u', 'i', 'o', 'o', 'u', 'e', 'o', 'e', 'e', 'a', 'o', 'e', 'a']


