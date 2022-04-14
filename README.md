# m1-setup
installing popular libraries on apple silicon 


## tensorflow:
here's a way to avoid interacting with conda mini-forge:
https://stackoverflow.com/questions/65383338/zsh-illegal-hardware-instruction-python-when-installing-tensorflow-on-macbook/68214296#68214296


## pytorch:
should just work with `pip3 install torch`. 
See: https://github.com/pytorch/pytorch/issues/56333


## scikit-learn
usually the issue is I can't build `scipy`, here's a fix for that:
https://github.com/scipy/scipy/issues/13409
