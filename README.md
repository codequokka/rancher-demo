# Rancher-quickstart-manual-setup

```console
$ sudo apt install -y virtualbox
$ sudo apt install -y vagrant
```

```console
$ vagrant up

$ python3 -m venv .venv
$ source .venv/bin/activate
$ pip install -r ./requirements.txt

$ ansible-galaxy install -r ./requirements.yml
$ ansible-playbook -i hosts ./playbooks/setup-rancher.yml
```

access https://192.168.33.11/

https://github.com/ibrokethecloud/core-bundles