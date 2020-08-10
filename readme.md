<p align="center">
<a href="https://dscommunity.in">
	<img src="https://github.com/Data-Science-Community-SRM/template/blob/master/Header.png?raw=true" width=80%/>
</a>
  <h2 align="center">Handwriting Synthesis</h2>
<h4 align="center">Implementation of the handwriting synthesis experiments in the paper <a href="https://arxiv.org/abs/1308.0850">Generating Sequences with Recurrent Neural Networks</a> by Alex Graves.  The implementation closely follows the original paper, with a few slight deviations, and the generated samples are of similar quality to those presented in the paper.</h4>
</p>

## Requirements

* matplotlib>=2.1.0
* pandas>= 0.22.0
* scikit-learn>=0.19.1
* scipy>=1.0.0
* svgwrite>=1.1.12
* tensorflow==1.6.0
* numpy==1.16.4

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



## Contributors


<table>
<tr align="center">
<td>
Paras Rawat

<p align="center">
<img src = "https://github.com/Data-Science-Community-SRM/template/blob/master/logo-light.png?raw=true"  height="120" alt="Your Name Here (Insert Your Image Link In Src">
</p>
<p align="center">
<a href = "https://github.com/TrizteX"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
<a href = "https://www.linkedin.com/in/paras-rawat-427a52174/">
<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36"/>
</a>
</p>
</td>


<td>
Siddharth Sudhakar

<p align="center">
<img src = "https://github.com/Data-Science-Community-SRM/template/blob/master/logo-light.png?raw=true"  height="120" alt="Your Name Here (Insert Your Image Link In Src">
</p>
<p align="center">
<a href = "https://github.com/siddharth271101"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
<a href = "https://www.linkedin.com/in/siddharth-sudhakar/">
<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36"/>
</a>
</p>
</td>

</tr>
</table>


## License
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

<p align="center">
	Made with :heart: by <a href="https://dscommunity.in">DS Community SRM</a>
</p>

