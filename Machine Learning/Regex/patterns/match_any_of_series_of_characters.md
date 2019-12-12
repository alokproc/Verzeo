---
title: "Match Any Of A Series Of Options"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match any of a series of options in Python."
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
# Find any of fox, snake, or bear
re.findall(r'fox|snake|bear', text)
```




    ['fox', 'bear']


