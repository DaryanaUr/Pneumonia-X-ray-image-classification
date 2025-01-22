### Sometimes mistakes can happen and it is best to leave them encapsulated in virtual environments.
________________________________________
### We need to create the environment at the CMD
conda create --name xray_env python=3.9
conda activate xray_env

### Then, you need to install the libraries
pip install os tensorflow matplotlib seaborn pandas numpy scikit-learn opencv-python jupyter tqdm

### Install the Jupyter kernel in the virtual environment
pip install ipykernel
python -m ipykernel install --user --name=xray_env --display-name "Python (xray_env)"

📌
When you open the notebook, select the Python kernel (xray_env) from the Kernel > Change kernel menu!
