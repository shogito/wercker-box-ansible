# wercker-box-ansible

### これはなに？
Werckerでansible-playbooの自動テストを実施するためのBOX


### environment variables
* ANSIBLE_PATH: /opt/ansible/bin
    container内のansibleがインストールされるpath

### やってること
* wercker-labs/dockerを継承
* docker-enterをインストール
* ansibleの公式が提供しているcentos7-ansibleとubuntu14.04-ansibleをpull
* box自身にもansibleをインストール

### TODO
* boxとcontainerのansibleインストール先を合わせる
* centos6/ubuntu12.04にも対応したい
* ansibleのlocal実行しか対応していないのでsshでのansible検証が出来るようにしとく

