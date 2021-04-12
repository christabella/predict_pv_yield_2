# Intro
Early experiments on predicting solar PV yield using satellite imagery, deep learning and optical flow.


# Installation

```
conda env create -f environment.yml
sudo apt install libgl1-mesa-glx  # required for OpenCV
conda activate predict_pv_yield
```

## Neptune Jupyter extension (Optional)
Follow the [Neptune docs](https://docs.neptune.ai/getting-started/installation/install-neptune-notebooks-jupyter-extension):
```
pip install neptune-notebooks
jupyter nbextension enable --py neptune-notebooks
```
If not installed already,
```
conda install -c conda-forge neptune-client
conda install -c anaconda psutil
```

# Using Neptune
Either click "Activate" on the Jupyter notebook menu bar, or manually set the env vars, e.g.:
```
export NEPTUNE_API_TOKEN=<API_TOKEN>
export NEPTUNE_PROJECT="OpenClimateFix/forecasting-satellite-images"
export NEPTUNE_NOTEBOOK_ID=...
export NEPTUNE_NOTEBOOK_PATH=...
```
