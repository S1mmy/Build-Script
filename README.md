# Build-Script
Before running libspn:

```
!git clone --single-branch --branch feature/em_sum_sampling https://github.com/jostosh/libspn.git

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