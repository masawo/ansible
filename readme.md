## ubuntuでansibleを使って以下を構築する

@ Ubuntu 13.04

- rbenv
- ruby 2.0.0 (↑を使って)
- Rails開発に必要なもの
    - mysql, redis, memcached, mongodb

## vagrantの準備

以下にならって  
http://yteraoka.github.io/ansible-tutorial/#server-setup-using-vagrant

## ansibleの最新版を入れる

    sudo apt-get install software-properties-common
    sudo add-apt-repository ppa:rquillo/ansible
    sudo apt-get update
    sudo apt-get install ansible -y

## playbook実行

    ansible-playbook -i hosts site.yml -vv

## 参考

- http://yteraoka.github.io/ansible-tutorial/
- http://qiita.com/dayflower/items/a07762f53e19850ea43e
