# ZCA-Whitening-Python
ZCA Whitening in Python



#### Example

```python
from zca import ZCA
import numpy as np

N = 100
K= 4

data = np.random.rand(N, K)

zca = ZCA()

# Separate fit and transform
zca.fit(data)
data_zca = zca.transform(data)

# Or joint
data_zca = zca.fit_transform(data)
```