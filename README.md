# worldcereal-yield

![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python 3.12](https://img.shields.io/badge/Python-3.12-blue.svg)

Repository for WorldCereal yield prediction work.

**Contents**
- Jupyter notebook: `Ukraine/ARYA_Ukraine.ipynb`
- Conda environment: `environment.yml`

**Install**
1. Install Miniconda or Anaconda.
2. Create the environment:
   ```bash
   conda env create -f environment.yml
   ```
3. Activate it:
   ```bash
   conda activate arya_openeo
   ```
4. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

**Notebook Overview**
The notebook `Ukraine/ARYA_Ukraine.ipynb` contains the workflow for preparing and uploading yield-related data. At a high level it:
- Loads and inspects the input data.
- Performs preprocessing and feature preparation.
- Runs the upload/export steps needed to publish the resulting artifacts.

Open the notebook in Jupyter, run the cells top-to-bottom, and adjust paths or parameters as needed for your environment.

**Required Credentials**
The upload steps require credentials for the target platform/service. Set them before launching Jupyter, for example:
```bash
export OPENEO_URL="https://<your-openeo-endpoint>"
export OPENEO_USER="<your-username>"
export OPENEO_PASSWORD="<your-password>"
```

If your deployment uses a token instead, export it and follow the notebook instructions:
```bash
export OPENEO_TOKEN="<your-token>"
```
