---
title: "Match US and UK Spellings"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match US and UK spellings in Python."
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
text = 'It\s center and not centre.'
```

## Apply regex


```python
# Find any ISBN-10 or ISBN-13 number
re.findall(r'\bcent(?:er|re)\b', text)
```




    ['center', 'centre']


