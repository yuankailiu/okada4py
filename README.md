# okada4py
Okada implementation in Python

## Citation
This is a python implementation of the solution proposed by Okada in 1992. Please cite:

Okada, Y. (1992), Internal deformation due to shear and tensile faults in a half-space, Bulletin of the Seismological Society of America, 82(2), 1018–1040.

## Install okada4py:

### Compilation
```
export CC=gcc
python setup.py build
```

### Linking

Link in a user module directory (on MacOS it is usually in ~/Library/Python/3.7/lib/python/site-packages/):
```
python setup.py install --user
```
On some OS, it is sometimes better to run :
```
python setup.py install --user --prefix=
```

On a Linux distribution:
+ We must run the above first in the `base` conda env, then the module is put to: ~/.local/lib/pythonX.Y/site-packages/
+ Now can run `okada4py` in your `base` conda env.
+ Further, if you want to use `okada4py` in other conda envs, `conda activate that_specific_env` and run the above `setup.py` again in that specific env. This should do it!

