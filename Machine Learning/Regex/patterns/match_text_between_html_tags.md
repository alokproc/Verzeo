---
title: "Match Text Between HTML Tags"
author: "Chris Albon"
date: 2017-12-20T11:53:49-07:00
description: "Match text between HTML tags in Python."
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
text = '<p>The quick brown fox.</p><p>The lazy brown bear.</p>'
```

## Apply regex


```python
# Find any text between '<p>' and '</p>'
re.findall(r'<p>(.*?)</p>', text)
```




    ['The quick brown fox.', 'The lazy brown bear.']


