# Deep Reinforcement Learning Tutorial

Contains Jupyter notebooks associated with the [*Deep Reinforcement Learning Tutorial*](https://conferences.oreilly.com/artificial-intelligence/ai-ny/public/schedule/detail/59390) given at the O'Reilly 2017 NYC AI Conference. Slides from the presentation can be downloaded [here](https://drive.google.com/open?id=0BxZSPcA0DrkfNG9aSjYxM1RMVzQ).

Required Unity Environments can be downloaded [here](https://drive.google.com/drive/folders/0BxZSPcA0DrkfQ2pPWkRFQkNiTnc?usp=sharing). Download and unzip the .zip file associated with your OS (ie Linux, Mac, or Windows) and move each of the files within the unzipped folder (ie 2DBall, 3DBall, etc) to the root directory of this repository.

## Requirements
* Tensorflow (version 1.0+)
* Pillow
* Matplotlib
* numpy
* scipy
* Jupyter

To install dependencies, run:

`pip install -r requirements.txt`

or 

`pip3 install -r requirements.txt`

If your Python environment doesn't include `pip`, see these [instructions](https://packaging.python.org/guides/installing-using-linux-tools/#installing-pip-setuptools-wheel-with-linux-package-managers) on installing it.

## Training RL Agents

To launch jupyter, run:

`jupyter notebook` 

Then navigate to `localhost:8888` to access each training notebook.

To monitor training progress, run the following from the root directory of this repo:

`tensorboard --logdir='./summaries'`

Then navigate to `localhost:6006` to monitor progress with Tensorboard.

## Troubleshooting

### macOS Permission Error

If you recieve a permission error when attempting to launch an environment on macOS, run:

`chmod -R 755 *.app` 

### Filename not found

If you recieve a file-not-found error while attempting to launch an environment, ensure that the environment files are in the root repository directory. For example, if there is a sub-folder containing the environment files, those files should be removed from the sub-folder and moved to the root. 
