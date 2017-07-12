## A brief reminder on using colors

## Import 
```python
%matplotlib inline
import numpy as np
import matplotlib.pyplot as plt
from scipy import stats
```

## Use seaborn plotting defaults
```python
import seaborn as sns; sns.set()
```

## Use Colorbrewer for less than 10 groups
```python
sns.palplot(sns.color_palette(palette = 'colorblind', n_colors = 10))
```

## See what happens when you use Colorbrewer for more than 10 groups
```python
sns.palplot(sns.color_palette(palette = 'colorblind', n_colors = 20))
```

## Use "husl" for greater than 10 groups
```python
sns.palplot(sns.color_palette("husl", n_colors=40))

sns.color_palette("husl", n_colors=20)

from matplotlib.colors import rgb2hex
list(map(rgb2hex, sns.color_palette("husl", n_colors=20)))
```
