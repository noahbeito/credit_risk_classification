![CreditRisk](https://2csolution.it/wp-content/uploads/2020/01/Credit-risk-management.png)
# credit_risk_classification
Using a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
---
## Technologies
This analysis leverages python 3.7 with the following packages and libraries:
* [pandas](https://github.com/pandas-dev/pandas)
* [numpy](https://github.com/numpy/numpy)
* [pathlib](https://github.com/python/cpython/blob/main/Lib/pathlib.py)
* [scikit-learn](https://github.com/scikit-learn/scikit-learn)
* [imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn)
---
## Imports
```python
import numpy as np
import pandas as pd
from pathlib import Path
from sklearn.metrics import balanced_accuracy_score
from sklearn.metrics import confusion_matrix
from imblearn.metrics import classification_report_imbalanced

import warnings
warnings.filterwarnings('ignore')
```
---
## Contributors
[Noah Beito](https://www.linkedin.com/in/noah-beito/)
---
## License
[MIT](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt)
