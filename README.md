# notebooks

## Collection of Random Jupyter Notebooks served using JupyterHub

### To Run locally,

> Clone this repo

#### Install jupyterlab using pipenv

```bash
# To install pipenv, see: https://pypi.org/project/pipenv/

pipenv install jupyterlab
pipenv run jupyter lab

# Follow the link on displayed on terminal
```

To run dotnet and rust notebooks, their respective kernels are required.

### Jupyter Kernels for Rust and Dotnet

#### Rust Kernel through Evcxr

```bash
# See: https://github.com/google/evcxr/blob/master/evcxr_jupyter/README.md
rustup component add rust-src
sudo apt install jupyter-notebook cmake build-essential
cargo install evcxr_jupyter
evcxr_jupyter --install
```

#### Dotnet Kernel through dotnet interactive

```bash
# See: https://github.com/dotnet/interactive
dotnet tool install --global Microsoft.dotnet-interactive
dotnet interactive jupyter install
```