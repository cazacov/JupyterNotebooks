# JupyterNotebooks
Experiments with Jupiter Notebook as IDE

## Setup JupyterLab
Install with conda

```bash
conda install -c conda-forge jupyterlab
```

## Setup Julia

Create symbolic link to run Julia from terminal
```bash
sudo ln -s /Applications/Julia-1.3.app/Contents/Resources/julia/bin/julia /usr/local/bin/julia
```

To change default Julia packahes location:
```bash
nano ~/.zprofile
export JULIA_DEPOT_PATH=...
```

Install Julia kernel for Jupyter
```bash
julia
julia> using Pkg
julia> Pkg.add("IJulia")
julia> ^D
```

## Run

```bash
jupyter lab
```
