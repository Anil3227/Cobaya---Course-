# Cobaya 
Installation and Using Guide.

Cobaya, a code for Bayesian analysis in Cosmology: Installation and Using Guide
===================
Cobaya (code for bayesian analysis, and Spanish for Guinea Pig) is a framework for sampling and statistical modelling: it allows you to explore an arbitrary prior or posterior using a range of Monte Carlo samplers (including the advanced MCMC sampler from CosmoMC, and the advanced nested sampler PolyChord). The results of the sampling can be analysed with GetDist.

Its authors are Jesus Torrado and Antony Lewis.

The original web page [Cobaya Website](https://cobaya.readthedocs.io/en/latest/index.html) that is cited in this document.

Visit https://himanshu1729-cosmo.github.io/tutorials/ for Windows/ linux in detail.

===================

First Download and Install Anaconda / Just use code below to install mini-conda quickly
```
mkdir -p ~/miniconda3
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh -o ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh
source ~/miniconda3/bin/activate
conda --version     (check if installed)
```




Create Virtual Environment 
```
conda create --name cobaya_env python=3.10 --platform osx-arm64
conda activate cobaya_env
python -m pip install --upgrade pip
conda install -c conda-forge openmpi mpi4py
```

install Cobaya and check Installation
```
python -m pip install cobaya --upgrade
python -c "import cobaya; print('Cobaya imported successfully!')"
python -c "import cobaya; print(cobaya.__version__)"

```
Make Cobaya working directory 
```
mkdir ~/cobaya
cobaya-install cosmo -p ~/cobaya
cobaya-install planck_2018_highl_plik.TTTEEE
cobaya-install bicep_keck_2018

mkdir ~/cobaya/chains
python -m pip install PySide6 (GUI tools)
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







