### Sometimes mistakes can happen and it is best to leave them encapsulated in virtual environments.
________________________________________
### We need to create the environment using our Anaconda Prompt
conda create --name xray1_env python=3.9
conda activate xray1_env

### Then we need the following tools from NVIDIA: 
conda install cudatoolkit=11.2 cudnn=8.1 -c=conda-forge

I'm using Python 3.9 in this environment because I need Tensorflow 2.7, check the following link to watch the table about GPU support:
https://docs.anaconda.com/working-with-conda/applications/tensorflow/
https://www.tensorflow.org/install/source_windows?hl=es-419#gpu

### You need to install the libraries
conda install tensorflow-gpu=2.7
pip install tensorflow==2.7
pip install os matplotlib seaborn pandas numpy scikit-learn opencv-python tqdm

### Install the Jupyter kernel in the virtual environment
pip install ipykernel
python -m ipykernel install --user --name=xray_env --display-name "Python (xray1_env)"

📌
When you open the notebook, select the Python kernel (xray1_env) from the Kernel > Change kernel menu!

### At the end: 
conda deactivate
