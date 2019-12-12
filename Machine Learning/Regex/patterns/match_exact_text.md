---
title: "Match Exact Text"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match exact text in Python."
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
# Find all instances of the exact match 'The'
re.findall(r'The', text)
```




    ['The']


