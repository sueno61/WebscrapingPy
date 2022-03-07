# ネイティブ環境 (not docker) でwebscraping using python

## Python library
- pandas, Pillow
- bs4, selenium, requests

## chromedriver
chromeのバージョンに合わせたドライバーをインストールすること  
＜以下、ubuntuの場合＞

### (1) chromeのバージョン確認
- chrome version.  99.0.4844.51  *ubuntu latest

### (2) バージョンに合わせたドライバーのインストール  
ダウンロード
```
    cd /tmp/
    curl -O https://chromedriver.storage.googleapis.com/99.0.4844.51/chromedriver_linux64.zip
```
解凍
```
    unzip chromedriver_linux64.zip
    ls -l
```
コピー（インストール）
```
    sudo mv chromedriver /usr/local/bin/
```
動作確認
```
    which chromedriver 
```
あとしまつ
```
    rm chromedriver_linux64.zip
```