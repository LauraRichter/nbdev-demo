---
jupyter:
  jupytext:
    formats: ipynb,py:light,md
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.14.1
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
---

# example

> First example

```python
#| default_exp example
```

```python
#| export
import matplotlib.pylab as plt
import numpy as np
import pandas as pd
```

```python
#| export

def simulate_data():
    x = np.arange(24)
    y = x ** 2
    return x, y
```

```python
x, y = simulate_data()
plt.plot(x, y)
```

```python
n = 15
plt.plot(np.random.randn(n))
print('plot!')
```

```python
df = pd.DataFrame({'x': x, 'y': y})
df
```

```python
#| hide
import nbdev; nbdev.nbdev_export()
```

```python

```
