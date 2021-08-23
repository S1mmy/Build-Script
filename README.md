# Build-Script
Programme basieren auf https://github.com/jostosh/libspn/blob/feature/em_sum_sampling

Before running libspn:

```
!git clone --single-branch --branch dspn_cont_gd https://github.com/jostosh/libspn.git

!pip install tensorflow-probability==0.8.0
!pip install tensorflow-gpu==1.15
!pip install scipy==1.2.2
!pip install colorama
!pip install GitPython
!ln -s /usr/local/lib/python3.7/dist-packages/tensorflow_core/libtensorflow_framework.so.1 /usr/local/lib/python3.7/dist-packages/tensorflow_core/libtensorflow_framework.so

%cd libspn
!python3 setup.py clean
!python3 setup.py build
```

After that:

```
%cd libspn
import libspn as spn
import tensorflow as tf
tf.logging.set_verbosity(tf.logging.ERROR)

import numpy as np
%matplotlib inline
import matplotlib.pyplot as plt
import scipy as scp
```