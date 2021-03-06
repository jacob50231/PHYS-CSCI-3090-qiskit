# Setup

1. Go to [this link](https://docs.anaconda.com/anaconda/install/) and follow the directions to install for your operating system.
2. For Mac/Linux open your terminal. For PC open up the "Anaconda Navigator" application go to environments, click the green play button, and then click "Open Terminal."
3. Navigate to the directory of this repository (for example `cd ~/Desktop/PHYS-CSCI-3090-qiskit/`)
4. Create environment from environment.yml file: `conda env create -f environment.yml`
5. Activate environment: `conda activate Quantum_Computing`

At this point, you can just activate Jupyter Notebook by typing the command `jupyter-notebook` into your shell and run simulations locally. If you'd like to set up to run on actual IBM quantum devices follow the steps below.

1. Create an account at: https://quantum-computing.ibm.com/
2. Copy API token from the dashboard
3. Somewhere in a Jupyter-Notebook or python script, evaluate the following code:


   `import IBMQ` <br>
   `IBMQ.save_account('your-token-here')`
