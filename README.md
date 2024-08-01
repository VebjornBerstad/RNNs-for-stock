# Stock predictions using recurrent neural networks

## Description

This is a student project for the class "ACIT4620 - Computational Intelligence" at Oslomet (Oslo Metropolitan University).

## Installation

### Requirements

1) The project requires Python 3.10 or higher to be installed, see [Python's homepage](https://www.python.org/downloads/) for instructions.
2) CUDA 11.6 or higher also needs to be installed, see the nVidia [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit-archive) for instructions on downloading the right version, along with the appropriate installation guides for your operating system ([Windows](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html), [Linux](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)).
3) Download the project code with git into a suitable folder.
4) Run `pip install .` for deployment or `pip install -e .[dev]` for development.
5) Additionally [install PyTorch](https://pytorch.org/get-started/locally/) matching your operating system and CUDA version, e.g: `pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu116`
6) For deployment, install pre-commit by running `pre-commit install`.

#### TA-lib
To install TA-lib,
1) Got to [UCI.edu](https://www.lfd.uci.edu/~gohlke/pythonlibs/#ta-lib) and find the version for your system.
2) Download the file and put it in your working root
3) Run `pip install [filename]` (in the case of a Windows 64 bit, python 3.8 run `pip install pip .\TA_Lib-0.4.24-cp38-cp38-win_amd64.whl`)



## Usage

The main code which trains the neural networks can be run with `python -m stockpred.main`.

Running experiments can be done with `python -m stockpred.experiments.[name of experiment]`. They are found in the `stockpred/experiments` folder.
