---
title: "Match A Word"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match a word in Python."
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
# Find any word of three letters
re.findall(r'\b...\b', text)
```




    ['The', 'fox', 'the']


