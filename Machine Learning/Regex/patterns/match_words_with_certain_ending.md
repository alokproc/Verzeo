---
title: "Match Words With A Certain Ending"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match words with a certain ending in Python."
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
text = 'Capitalism, Communism, Neorealism, Liberalism'
```

## Apply regex


```python
# Find any word ending in 'ism'
re.findall(r'\b\w*ism\b', text)

# Specific:
# \b     - start of the word
# \w*    - a word of any length
# ism\b  - with 'ism'at the end
```




    ['Capitalism', 'Communism', 'Neorealism', 'Liberalism']


