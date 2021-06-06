# Ubuntu に Jupyer lab をインストールする

```
sudo apt-get update

sudo apt-get install -y sudo wget vim curl gawk make gcc apt-utils python3-pip

sudo pip install --upgrade pip

sudo pip install pandas_datareader

sudo pip install jupyter

sudo pip install jupyterlab

jupyter lab --allow-root -LabApp.token='' --ip=0.0.0.0 --no-browser

```
