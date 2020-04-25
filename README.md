# Generative Adversarial Networks: Face Synthesis

Implementation of a GAN for face synthesis using a celebrity image dataset.

## Setup

```shell
$ python -m venv venv
$ pip install -r requirements.txt
```

To start a new Jupyter Notebook kernel:

```shell
$ ipython kernel install --name "local-venv" --user
```

To list all kernels:

```shell
$ jupyter kernelspec list
```

To remove a kernel:

```shell
$ jupyter kernelspec uninstall unwanted-kernel
```

### To setup jupyter notebook extensions

`pep8` package is required for auto-linting in the notebook.

```shell
$ pip install -e jupyter_contrib_nbextensions     # For pip
$ conda install -c conda-forge jupyter_contrib_nbextensions # For Anaconda
$ jupyter contrib nbextension install --user
$ pip install pep8                                # For pip, required for auto-linting
$ conda install -c anaconda pep8                  # For Anaconda, required for auto-linting
```

### To setup Jupyter Notebook themes

We use [dunovank/jupyter-themes](https://github.com/dunovank/jupyter-themes)

```shell
$ pip install --upgrade jupyterthemes             # For pip
$ conda install -c conda-forge jupyterthemes      # For Anaconda
$ jt -t chesterish -T -f roboto -fs 12 -cellw 95% # Sets theme to chesterish, enables toolbar, sets font to robot, sets fontsize to 12, set cell width to 95% of screen
```

### To log into Server and set up a jupyter notebook instance

1.  `$ ssh username@server_ip_addr`
2.  Install anaconda in the server
3.  `$ conda create -n env_name python=3.7`
4.  `$ conda activate env_name`
5.  `$ conda install python_package_name`
6.  `$ conda info --env`
7.  `$ conda list`
8.  `$ ssh -L 8000:localhost:8888 username@your_server_ip` # From local machine terminal
9.  `$ jupyter notebook --no-browser`
10. On your local machine, go to `http://localhost:8000` and enter token from server.
11. `!conda list` # From inside the jupyter notebook test modules

## Conda environment

Note: To export current conda env

`$ conda-env  export -n your_env_name > your_env_name.yml`

To create new environment using yml configuration file run:

`$ conda-env create -n new_env -f=\path\to\base.yml`

## Data

## Preprocessing Data

## Activation functions used

![](img/sigmoid.png)

![](img/sigmoid_derivative.png)

![](img/relu.png)

![](img/relu_derivative.png)

![](img/tanh.png)

![](img/tanh_derivative.png)

## Results of training and testing with sklearn's train_test_split
