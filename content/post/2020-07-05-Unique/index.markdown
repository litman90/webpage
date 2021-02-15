---
title: Unique
subtitle: 
date: 2020-07-05
author: "Matias Andina"
tags: ["fun", "python", "R"]
mathjax: true
---

I have experienced a few explosions here and there. Yes, it's me not reading the docs. But it's also me, assuming that verbs mean one thing and not another. Let's do some `unique` operations in different languages.

### The MATLAB way

```
>> unique([3, 3, 3, 90, 10])

ans =

3 10 90
```

### The Python way

```
>>> import numpy as np
>>> np.unique([3, 3, 3, 90, 10])
array([ 3, 10, 90])
```

### The R way


```r
unique(c(3,3,3, 90, 10))
```

```
## [1]  3 90 10
```

This is what I would expect. I want the unique values, **without** the sorting. If I wanted to sort, I would do:


```r
sort(unique(c(3,3,3, 90, 10)))
```

```
## [1]  3 10 90
```

Maybe this is just me and R is the odd (read intuitive) ball here, but 🤷...
