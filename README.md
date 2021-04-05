# notebooks

## Collection of Random Jupyter Notebooks served using JupyterHub

### To Run locally,

> Clone this repo

#### Install Jupyter-notebook and build tools

```bash
sudo apt install jupyter-notebook cmake build-essential

# Install Python3 and pipenv if not already installed
# sudo apt install python3-dev python3-dev virtualenv python3-setuptools pipenv
```

#### Install jupyterlab using pipenv

```bash
# To install pipenv, see: https://pypi.org/project/pipenv/

# From this repo dir,
pipenv install jupyterlab
pipenv run jupyter lab

# Follow the link on displayed on terminal to open jupyterlab
```

To run dotnet and rust notebooks, their respective kernels are required.

### Jupyter Kernels for Rust and Dotnet

#### Rust Kernel through Evcxr

```bash
# See: https://github.com/google/evcxr/blob/master/evcxr_jupyter/README.md
rustup component add rust-src
cargo install evcxr_jupyter
evcxr_jupyter --install
```

#### Dotnet Kernel through dotnet interactive

```bash
# See: https://github.com/dotnet/interactive
dotnet tool install --global Microsoft.dotnet-interactive
dotnet interactive jupyter install
```