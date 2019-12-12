---
title: "Match A Symbol"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match a symbol in Python."
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
text = '$100'
```

## Apply regex


```python
# Find all instances of the exact match '$'
re.findall(r'\$', text)
```




    ['$']


