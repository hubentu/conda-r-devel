## R development version (4.0.0) conda recipe
* Copied from https://github.com/conda/conda-recipes/blob/master/r-base
* Only tested on ubuntu 18.04

## Howto
* Create r-devel env
```sh
git clone https://github.com/hubentu/conda-r-devel.git
cd conda-r-devel
conda create -n r-devel
conda activate r-devel
```

* Build and install
From source
```sh
conda install conda-build
conda build .
conda install --use-local path/to/r-devel
```

Or just install the compiled version from ubuntu 18.04
```sh
conda install --use-local r-devel-4.0.0-0.tar.bz2
conda install readline
```

* Use R 4.0
```sh
R --version
```
