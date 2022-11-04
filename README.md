# DSCoV-NapariWorkshop

This repo hosts code and slides used for the DSCoV workshop on the napari image viewer on 11-04-22. In this repo you will find:

* **demo.ipynb**: Jupyter Notebook that you can run and follow along with the demostration.
* **load_env.sh**: **Oscar/Open OnDemand Desktop ONLY !!** Load the necessary modules to run the demo in Open OnDemand desktop on Oscar.
* **requirements.txt**: All dependencies needed to run the demo with your own venv/conda environment.
* **images/**: directory: Images used for demo and readme.

## Run the demo in Open OnDemand on Oscar (Recommended):

#### First, launch a desktop instance in Open OnDemand

* Go to [Open OnDemand](https://ood.ccv.brown.edu) 
* Click on "Desktop"
* Choose a GPU instance, none GPU instances would work but `napari` runs faster on GPUs
* Click "Launch"
* When the instance is ready, launch the remote desktop in your browser

#### Then, launch the demo Juypyter notebook

* Start a terminal in the desktop environment
* Clone this repo [https://github.com/brown-ccv/DSCoV-NapariWorkshop](https://github.com/brown-ccv/DSCoV-NapariWorkshop)
* In the cloned repo, type `bash load_env.sh`
* You may need to load the conda module with: `module load anaconda/2022.05`;     
  After loading the module, `conda init bash`
* Activate the conda environment `conda activate /gpfs/runtime/opt/DSCoV_env`
* Launch Jupyter notebook, `jupyter notebook` (Lab might not work)
* Open `demo.ipynb`, and execute each cell

## Run the demo on your own computer

* Clone this repo [https://github.com/brown-ccv/DSCoV-NapariWorkshop](https://github.com/brown-ccv/DSCoV-NapariWorkshop)
* Set up a virtual environment with either of the two methods below. Because `napari` requires `pyQT`, which might cause some issues with `pip install`, especailly on M1 Macs. We recommend using `conda` to set up the environment.

#### (Option 1) Set up a conda environment (Recommended)

* Create a conda environment using `conda create -f environment.yml`
* Activate the enviornment using `conda activate napari_env`

#### (Option 2) Set up a virtual environment using `venv`

* Create a virtual environment using `venv`: `python -m venv .venv`

If you are on MacOS/Linux:
* Activate the environment `source .venv/bin/Scripts/activate`

If you are on Windows:
* Activate the environment using CMD `.venv\Scripts\activate.bat`
* Or, activate the environment using PowerShell `.venv\Scripts\activate.ps1`

* Install all dependencies `pip install -r requirements.txt`

## After activating your virtual environment

* Launch Jupyter notebook/lab, `jupyter notebook` or `jupyter lab`
* Open `demo.ipynb`, and execute each cell

