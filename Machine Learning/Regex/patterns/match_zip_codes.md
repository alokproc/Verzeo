---
title: "Match ZIP Codes"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match ZIP codes in Python."
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
text = '3829 South Ave Street, Pheonix, AZ 34923'
```

## Apply regex


```python
# Find any ISBN-10 or ISBN-13 number
re.findall(r'[0-9]{5}(?:-[0-9]{4})?', text)
```




    ['34923']


