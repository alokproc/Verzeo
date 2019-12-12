---
title: "Match Times"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match times in Python."
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
text = 'Chris: 12:34am. Steve: 16:30'
```

## Apply regex


```python
# Find any text that fits the regex
re.findall(r'([0-1]\d:[0-5]\d)\s*(?:AM|PM)?', text)
```




    ['12:34', '16:30']


