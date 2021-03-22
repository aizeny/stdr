# STDR - Spectral Top Down Reconstruction
Code for the paper "Spectral Top-Down Recovery of Latent Tree Models" (https://arxiv.org/abs/2102.13276)


## Installing
You should install the package using pip. cd inside the `stdr` folder and run 
```
pip install .
```
Now if you want to import the spectraltree package, for example for an experiment, you can simply run
```
import spectraltree
```

## Testing
To run the test suite, cd to `stdr` and run
```
python -m unittest discover
```
To run a specific module:
```
python -m unittest tests.test_stdr
```


## Installing RAxML
In order to use RAxML (A. Stamatakis: "RAxML Version 8: A tool for Phylogenetic Analysis and Post-Analysis of Large Phylogenies". In Bioinformatics, 2014),
the RAxML executible should be placed in 
spectraltree\libs\raxmlHPC_bin\
For macOS the file should be named: raxmlHPC-macOS
For Windows the file should be named: raxmlHPC-SSE3.exe
For Linux the file should be named: raxmlHPC-SSE3-linux


For further details, look in spectraltree\raxml_reconstruction.py and https://cme.h-its.org/exelixis/web/software/raxml/

## Documentation
Run
```
python setup.py build_sphinx
```
(You can also go into the `docs` folder and run `make html`). Then open `docs/_build/html/index.html` in a browser.
