# SarXarray

`SarXarray` is an `Xarray` extension to process coregistered Single Look Complex (SLC) image stacks acquired by Synthetic Aperture Radar (SAR). It utilizes `Xarray`’s support on labeled multi-dimensional datasets to stress the space-time character of the SLC SAR stack. It also takes the benefits from `Dask` to perform lazy evaluations of the operations.

## Installation

First, clone this repository to your local file system:

```bash
git clone git@github.com:MotionbyLearning/sarxarray.git
```

It is strongly recommended to install `sarxarray` under an independent Python environment, e.g. an independent [conda](https://docs.conda.io/en/latest/miniconda.html) environment. If `conda` is already installed in your system, you can create a new environment by:

```bash
conda create -n sarxarray_demo python=3.10
```

A new environment named `sarxarray_demo` will be created. Then you can activate it by:

```bash
conda activate sarxarray_demo
```

After creating a new environment, you can install `SarXarray` using `pip`:

```bash
cd sarxarray
pip install .
```

## Usage example

An [example Jupyter Notebook](examples/demo_sarxarray.ipynb) is available to demonstrate the usage of `SarXarray`.

Note that to execute the Jupyter Notebook, you may need to install two more packages:

- `jupyterlab`
- `matplotlib`

You can install them in your current `conda` environment by:

```bash
conda install jupyterlab matplotlib
```

After installation, execute the notebook in a JupyterLab session, which can be started by running `jupyterlab` command in your command line:

```bash
jupyter-lab
```

A new tab will be opened in your default browser. If it does not open automatically, you need to find the URL of the JupyterLab session in your command line, then open it manually.

In this tab, you will see the file structure inside the `sarxarray` directory. You can open the example Notebook at `examples/demo_sarxarray.ipynb` and execute it.
