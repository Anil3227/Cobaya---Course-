## Lollipop Likelihood Installation


See the [Lollipop documentation](https://github.com/planck-npipe/lollipop) for details.

```bash
# Open the code folder; replace this path with your own
cd /Users/anilkandel/Documents/cobaya/code

# Download Lollipop and enter its folder
git clone https://github.com/planck-npipe/lollipop.git
cd lollipop

# Install the package and likelihood data
pip install -e .
cobaya-install planck_2020_lollipop.lowlE
```

## Hillipop Likelihood Installation


See the [Hillipop documentation](https://github.com/planck-npipe/hillipop) for details.

```bash
# Open the code folder; replace this path with your own
cd /Users/anilkandel/Documents/cobaya/code

# Download Hillipop and enter its folder
git clone https://github.com/planck-npipe/hillipop.git
cd hillipop

# Install the package and likelihood data
pip install -e .
cobaya-install planck_2020_hillipop.TTTEEE
```


## WMAP likelihood

See the [WMAP likelihood documentation](https://github.com/HTJense/pyWMAP) for details.

```bash
# Open the code folder; replace this path with your own
cd /Users/anilkandel/Documents/cobaya/code

git clone https://github.com/HTJense/pyWMAP
cd pyWMAP

pip install -e .
```


# Atacama Cosmology Telescope (ACT) DR6 CMB-Only Likelihood Installation

See the [ACT DR6 CMB-only likelihood documentation](https://github.com/ACTCollaboration/DR6-ACT-lite) for details.

```bash
# Open the code folder; replace this path with your own
cd /Users/anilkandel/Documents/cobaya/code

# Download ACT DR6 and enter its folder
git clone https://github.com/ACTCollaboration/DR6-ACT-lite.git
cd DR6-ACT-lite

# Install the package and likelihood data
pip install -e .
cobaya-install act_dr6_cmbonly

# Planck dataset cut at the ACT multipole
cobaya-install act_dr6_cmbonly.PlanckActCut

```


