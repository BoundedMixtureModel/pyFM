# Factorization Machines in Python

Cython bindings to Steffen Rendle’s [LibFM](http://www.libfm.org/), a c++ library implementing factorization machines for collaborative filtering and recommendation.

Factorization machines (FM) are a generic approach that allows to mimic most factorization models by feature engineering. This way, factorization machines combine the generality of feature engineering with the superiority of factorization models in estimating interactions between categorical variables of large domain.

compat.py implements an sklearn base.BaseEstimator to allow this library to be incorporated into a broader workflow in python.

## Dependencies
* cython >= 0.17 (previous versions will not work)
* numpy
* pandas
* libFM source

## Installation
1. Download libFM source code from http://www.libfm.org/
2. Extract the source (```wget http://www.libfm.org/libfm-1.30.src.tar.gz```)
3. ```cp -r libfm-1.30.src/src pyLibFM/minifm/```
4. ```cd pylibfm``` 
5. ```python setup.py install``` 


## License
From libfm's license.txt:
1. This software is free of charge for academic purposes. Please contact the author if you want to use this software for commercial purposes.
2. You are not allowed to redistribute this software or its source code.
3. Please acknowledge this software if you publish results produced with this software by citing the paper "Steffen Rendle. Factorization machines with libFM. ACM Trans. Intell. Syst. Technol., 3(3), May 2012." 