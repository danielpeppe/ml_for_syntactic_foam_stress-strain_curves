## Setup

1. Setup your Python environment using venv (Windows):
    ```sh
    py -m venv .venv
    ```
2. Activate the environment in the terminal:
    ```sh
    .\.venv\Scripts\activate
    ```
3. Install dependencies:
    ```sh
    py -m pip install -r requirements.txt
    ```
    If you don't have an NVIDIA GPU, just install PyTorch for CPU:
    ```sh
    py -m pip install torch
    ```    
    Otherwise, you should install PyTorch for GPU (make sure you have the necessary drivers installed for CUDA):
    ```sh
    py -m pip install torch --index-url https://download.pytorch.org/whl/cu124
    ```

## Usage

```main_notebook.ipynb``` is the main Jupyter notebook which calls the functions included in the 'my_utils' folder. This includes data pre-processing, model selection and configuration, model training, validation, testing, saving and loading.

## Citation

If you use this work in academic or industrial research, please cite:

> Ferguson, E., Oggioni, F., Peppe, D., Whiteside, S., Fieldsend, H., & Tasdemir, B. (2026).  
> *The influence of volume fraction on the compressive behaviour of a polymeric syntactic foam: From manufacturing to machine learning-based modelling*.
> Materials Today Communications, 50, 114339.  
> https://doi.org/10.1016/j.mtcomm.2025.114339

A machine-readable citation is also provided in [`citation.cff`](./citation.cff) for use with GitHub and reference managers.
