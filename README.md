# AlphaGenomeWorkshop

This repository contains a modified jupyter notebook for Google DeepMind AlphaGenome API. Use subjected to AlphaGenome API terms of service - please see the corresponding pdf document in the repository.

# Creating the environment

git clone -b main https://github.com/maxplanck-ie/AlphaGenomeWorkshop.git

cd AlphaGenomeWorkshop

conda env create -f alphagenome.yaml

conda activate alphagenome

conda install ipykernel -y

python -m ipykernel install --user --name alphagenome --display-name "alphagenome"


# Open Visual Studio Code (or download it if you don't have it)

https://code.visualstudio.com/download

From Visual Studio Code under View -> Extensions install Google Colab

Install VS Code.
Install the Colab extension from either the Visual Studio Marketplace or Open VSX.
Open or create a notebook file.
When prompted, sign in.
Click Select Kernel > Colab > New Colab Server.

# How to get started with Google Colab

Go to https://colab.research.google.com/ , log in with your google account
Under the secrets tab create a new API Key ALPHA_GENOME_API_KEY


# Clone this repository

git clone git@github.com:maxplanck-ie/

Open the repository in quick_start.ipynb replace

dna_model = dna_client.create(colab_utils.get_api_key())
with
dna_model = dna_client.create(ALPHA_GENOME_API_KEY)




