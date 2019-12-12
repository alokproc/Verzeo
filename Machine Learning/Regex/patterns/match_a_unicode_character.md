---
title: "Match A Unicode Character"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match a unicode character in Python."
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
text = 'Microsoft™.'
```

## Apply regex


```python
# Find any unicode character for a trademark
re.findall(r'\u2122', text)
```




    ['™']


