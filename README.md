# m1-setup
Here are some of the fixes that helped in install popular ML/RL libraries on apple silicon.


## tensorflow:
here's a way to avoid interacting with conda mini-forge:
https://stackoverflow.com/questions/65383338/zsh-illegal-hardware-instruction-python-when-installing-tensorflow-on-macbook/68214296#68214296


## pytorch:
should just work with `pip3 install torch`. 
See: https://github.com/pytorch/pytorch/issues/56333


## scikit-learn
usually the issue is I can't build `scipy`, here's a fix for that:
https://github.com/scipy/scipy/issues/13409

## procgen
have to change CMakeLists.txt and compile from source, also change the C Compiler to Clang: 
https://github.com/openai/procgen/issues/69

## C Compiler to Clang:
Modify CMkaeLists.txt with the options here:
https://stackoverflow.com/questions/7031126/switching-between-gcc-and-clang-llvm-using-cmake
