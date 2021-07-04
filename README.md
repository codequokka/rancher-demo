# Rancher-quickstart-manual-setup

# Requirements(Ubuntu 20.04)
```console
$ sudo apt install -y virtualbox
$ sudo apt install -y vagrant
$ sudo apt install -y pytyhon3-pip
$ sudo apt install -y pytyhon3-venv
```

# Setup Rancher server
```console
$ git clone https://github.com/codequokka/rancher-demo
$ cd rancher-demo

$ vagrant up

$ python3 -m venv .venv
$ source .venv/bin/activate
$ pip install -r ./requirements.txt
$ ansible-galaxy install -r ./requirements.yml
$ ansible-playbook -i inventories/testing/hosts.ini ./playbooks/setup-rancher.yml
```

access https://192.168.33.11/