
# Handwriting Synthesis
Implementation of the handwriting synthesis experiments in the paper <a href="https://arxiv.org/abs/1308.0850">Generating Sequences with Recurrent Neural Networks</a> by Alex Graves.  The implementation closely follows the original paper, with a few slight deviations, and the generated samples are of similar quality to those presented in the paper.
## Requirements
matplotlib>=2.1.0
pandas>= 0.22.0
scikit-learn>=0.19.1
scipy>=1.0.0
svgwrite>=1.1.12
tensorflow==1.6.0
numpy==1.16.4
## Usage
Create a 'logs' folder before running, files are saved as usage_demo in img folder. Further instructions to run are in run.py
```
python run.py
```
![](img/usage_demo.svg)
  

A pretrained model is included, for training your own model:

## Model Training Instructions

In order to train a model, data must be downloaded and placed in this directory.

Follow the download instructions here http://www.fki.inf.unibe.ch/databases/iam-on-line-handwriting-database.

Only a subset of the downloaded data is required.  Move the relevant download data so the directory structure is as folllows:

```
data/
├── raw/
│   ├── ascii/
│   ├── lineStrokes/
│   ├── original/
|   blacklist.npy
```

Once this is completed, run `prepare_data.py` extract the data and dump it to numpy files.

To train the model, run `rnn.py`.  This takes a couple days on a single Tesla K80.

