# IMC 2025 - Domain Adaptation Workshop

This repository contains the code for the *Domain Adaptation* workshop held on 
September 1st, 2025 as part of the 9th Intelligent Maintenance Conference.

## 0 - Environment Setup

0. Clone this repository (or download it as a ZIP archive from GitHub and extract it):

```bash
git clone https://github.com/EPFL-IMOS/IMC2025_domain_adaptation.git
```


1. Install [uv](https://github.com/astral-sh/uv) using the [official instructions](https://github.com/astral-sh/uv?tab=readme-ov-file#installation). We use `uv` to manage Python version and packages.

2. Install Python 3.10 with `uv`:

```bash
uv python install 3.10
```

3. Navigate inside the cloned repository:
```bash
cd IMC2025_domain_adaptation
```

4. Install all the required packages automatically using `uv`:
```bash
uv sync
```

## 1 - Dataset Download

The datasets can be downloaded [here](https://drive.switch.ch/index.php/s/t8EsC0pBNbyxtqs).

## 99 - Organizers only

To re-create the official `uv` environment from scratch, use the following commands

```bash
# Install Python 3.10
uv python install 3.10

# Create imc2025 Python project
uv init imc2025

# Install PyTorch (must be 2.4.0 for PyTorch Geometric 2.6.1)
uv add torch==2.4.0
uv add torch_geometric==2.6.1

# Install utility libraries
uv add tqdm pandas numpy scipy seaborn matplotlib scikit_learn
```
