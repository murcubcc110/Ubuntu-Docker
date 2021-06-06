# Ubuntu に Jupyer lab をインストールする
 
```sh
# apt-get アップデート
sudo apt-get update

# 各パッケージインストール
sudo apt-get install -y sudo wget vim curl gawk make gcc apt-utils python3-pip

# pip アップデート
sudo pip install --upgrade pip

# pandas インストール
sudo pip install pandas_datareader

# jupyter インストール
sudo pip install jupyter

# jupyterlab インストール
sudo pip install jupyterlab

# jupyterlab 起動
jupyter lab --allow-root -LabApp.token='' --ip=0.0.0.0 --no-browser

```
