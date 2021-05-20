# Ubuntu へ Docker をインストールする
### 参考資料
* [Install Docker Engine on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
* [VirtualBox](https://qiita.com/HirMtsd/items/be1c8afe708e901e1100)
* [Ubuntuインストール](https://qiita.com/HirMtsd/items/225c20b77a7cd5194834)

### 手順
1. apt-get アップデート
    ```sh
    $ sudo apt-get update
    ```
2. パッケージインストール
    ```sh
    $ sudo apt-get install \
      apt-transport-https \
      ca-certificates \
      curl \
      gnupg \
      lsb-release
    ```
3. Docker の GPG key を追加
    ```sh
    $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg \
      | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
    ```
4. Docker（安定版）のリポジトリを設定します
    ```sh
    $ echo \
      "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
      $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    ```
5. 変更反映
    ```sh
    $ sudo apt-get update
    ```
6. Dockerインストール
    ```sh
    $ sudo apt-get install docker-ce docker-ce-cli containerd.io
    ```
7. Dockerバージョン確認
    ```sh
    $ sudo docker version
    ```
9. aa
10. 
    
    
    
    
    


