# flexget-python3-osmc


```
sudo apt-get install python3
```

configure alternatives as in (https://linuxconfig.org/how-to-change-from-default-to-alternative-python-version-on-debian-linux):

```
python --v
sudo update-alternatives --install /usr/bin/python python /usr/bin/python2.7 1
sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.4 2
update-alternatives --list python
sudo update-alternatives --config python
```

select 2 to set python default to python3

install pip, setuptools and virtualenv:
```
sudo apt-get install python3-pip
sudo pip3 install --upgrade setuptools
sudo pip3 install --upgrade virtualenv
```

install flexget as in (https://flexget.com/InstallWizard/Linux):

```
cd ~
virtualenv flexget
cd ~/flexget/
bin/pip install flexget
```

install transmissionrpc:

```
bin/pip install transmissionrpc
```

to run flexget without activation of the virtualenv:

```
~/flexget/bin/flexget -V
```
