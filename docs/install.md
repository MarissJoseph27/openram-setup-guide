# OpenRAM Installation

## Step 1: Clone OpenRAM

```bash
git clone https://github.com/VLSIDA/OpenRAM.git
cd OpenRAM
```


## Dependencies

- Git
- Make
- Python 3.5+
- Nix (recommended)


## Install Git, Make, Python

``` bash
sudo apt update
sudo apt install git make python3 python3-pip python3-venv
```


## Install Nix

```bash
curl -fsSL https://install.determinate.systems/nix | sh -s -- install
```


After installation, restart terminal.

---


## Setup Python Virtual Environment

```bash
cd OpenRAM
python3 -m venv openram_env
source openram_env/bin/activate
```


## Setup Python Dependencies

```bash
pip install -r requirements.txt
```

## Nix
Enter the Nix development environment with:
```bash
nix develop
```


