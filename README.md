# pycit
Framework for independence testing and conditional independence testing, with multiprocessing. Currently uses mutual information (MI) and conditional mutual information (CMI) as test statistics, estimated using k-NN methods. Also supports a routine for Markov blanket feature selection. Reports permutation-based p-values.

# Available test statistics
### Mutual Information Estimators
* ```ksg_mi```: k-NN estimator for continuous data
* ```bi_ksg_mi```: "bias-improved" k-NN estimator for continuous data
* ```mixed_mi```: k-NN estimator for discrete-continuous mixtures

### Conditional Mutual Information Estimators
* ```ksg_cmi```: k-NN estimator for continuous data
* ```bi_ksg_cmi```: "bias-improved" k-NN estimator for continuous data
* ```mixed_cmi```: k-NN estimator for discrete-continuous mixtures

### Other
* ```kl_entropy```: k-NN differential entropy estimator

# Example Usage 

### Independence Testing
```python
from test_statistics import *
from shuffle_tests import *
```

### Conditional Independence Testing
```python
from test_statistics import *
from shuffle_tests import *
```

### Markov Blanket Feature Selection
```python
from test_statistics import *
from shuffle_tests import *
```

### Differential Entropy Estimation
```python
from test_statistics import *
```

<!-- # Dependencies:
* Numpy
* Scipy
* scikit learn
* multiprocess -->

# References:
* Frenzel, S. and Pompe, B. (2007). Partial mutual information for coupling analysis of multivariate time series. Physical Review Letters, 99(20):204101.
* Gao, W., Kannan, S., Oh, S., and Viswanath, P. (2017). Estimating mutual information for discrete-continuous mixtures. In NIPS'2017.
* Gao, W., Oh, S., and Viswanath, P. (2018). Demystifying fixed k-nearest neighbor information estimators. IEEE Transactions on Information Theory, 64(8):5629–5661.
* Kozachenko, L. and Leonenko, N. (1987). Sample estimate of the entropy of a random vector. Problemy Peredachi Informatsii, 23(2):9–16.
* Kraskov, A., Stögbauer, H., and Grassberger, P. (2004). Estimating mutual information. Physical Review E, 69(6):066138.
* Runge, J. (2018). Conditional independence testing based on a nearest-neighbor estimator of conditional mutual information. In AISTATS'18.
* Yang, A., Ghassami, A., Raginsky, M., Kiyavash, N., and Rosenbaum, E. (2020). Model-Augmented Estimation of Conditional Mutual Information for Feature Selection. In UAI'2020.
