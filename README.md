# Cobaya 
Installation and Using Guide.

Cobaya, a code for Bayesian analysis in Cosmology: Installation and Using Guide
===================
Cobaya (code for bayesian analysis, and Spanish for Guinea Pig) is a framework for sampling and statistical modelling: it allows you to explore an arbitrary prior or posterior using a range of Monte Carlo samplers (including the advanced MCMC sampler from CosmoMC, and the advanced nested sampler PolyChord). The results of the sampling can be analysed with GetDist.

Its authors are Jesus Torrado and Antony Lewis.

The original web page [Cobaya Website](https://cobaya.readthedocs.io/en/latest/index.html) that is cited in this document. 

===================

Create Virtual Environment ( First Download and Install Anaconda)
```
conda create --name cobaya_env python=3.10 --platform osx-arm64
conda activate cobaya_env
python -m pip install --upgrade pip
conda install -c conda-forge openmpi mpi4py
```

install Cobaya
```
python -m pip install cobaya --upgrade
python -c "import cobaya; print('Cobaya imported successfully!')"
python -c "import cobaya; print(cobaya.__version__)"
mkdir ~/cobaya
cobaya-install cosmo -p ~/cobaya
mkdir ~/cobaya/chains
python -m pip install PySide6

```

Input file 
```
cobaya-cosmo-generator
```

After saving the .yaml file (e.g., test.yaml), run:
```
cobaya-run test.yaml
```
For Contour plots use text file (chain)
```
test.1.txt
```







