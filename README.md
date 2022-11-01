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
* Choose a non-GPU instance (e.g. 4 Cores, 15GB)
* Click "Launch"
* When the instance is ready, launch the remote desktop in your browser

#### Then, launch the demo Juypyter notebook

* Start a terminal in the desktop environment
* Clone this repo [https://github.com/brown-ccv/DSCoV-NapariWorkshop](https://github.com/brown-ccv/DSCoV-NapariWorkshop)
* In the cloned repo, type `bash load_env.sh`
* Launch Jupyter notebook/lab, `jupyter notebook` or `jupyter lab`
* Open `demo.ipynb`, and execute each cell

## Run the demo on your own computer

* Clone this repo [https://github.com/brown-ccv/DSCoV-NapariWorkshop](https://github.com/brown-ccv/DSCoV-NapariWorkshop)
* Create a virtual environment using `venv`: `python -m venv .venv` (you can also use Conda for this step as well)
* Activate the environment `source .venv/bin/Scripts/activate`
* Install all dependencies `pip install -r requirements.txt`
* Launch Jupyter notebook/lab, `jupyter notebook` or `jupyter lab`
* Open `demo.ipynb`, and execute each cell

