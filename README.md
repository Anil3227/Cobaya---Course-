# Cobaya---Course-
Installation and Using Guide.

Cobaya, a code for Bayesian analysis in Cosmology: Installation and Using Guide
===================
Cobaya (code for bayesian analysis, and Spanish for Guinea Pig) is a framework for sampling and statistical modelling: it allows you to explore an arbitrary prior or posterior using a range of Monte Carlo samplers (including the advanced MCMC sampler from CosmoMC, and the advanced nested sampler PolyChord). The results of the sampling can be analysed with GetDist.

Its authors are Jesus Torrado and Antony Lewis.

The original web page [Cobaya Website](https://cobaya.readthedocs.io/en/latest/index.html) that is cited in this document. 

Cobaya
===================

 Cobaya Installation for Mac
```
conda create --name cobaya_env python=3.10 --platform osx-arm64
conda activate cobaya_env
python -m pip install --upgrade pip
conda install -c conda-forge openmpi mpi4py
python -m pip install cobaya --upgrade
python -c "import cobaya; print('Cobaya imported successfully!')"
python -c "import cobaya; print(cobaya.__version__)"
mkdir ~/cobaya
cobaya-install cosmo -p ~/cobaya
mkdir ~/cobaya/chains
python -m pip install PySide6
cobaya-cosmo-generator
cobaya-run test.yaml
```




