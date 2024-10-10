# project path

## test python already installed

```bash
python3 --version
> Python 3.11.2
```

## install python and creating Virtual Environment with Python 3.11

** MISTAKE MAYBE ALL AS root**

```bash
#!/bin/bash \
sudo apt update \
&& sudo apt upgrade \
&& sudo apt-get --yes autoclean \
&& sudo apt-get --yes --auto-remove autoremove \
&& sudo apt-get --yes clean \
&& sudo rm --recursive --force /var/lib/apt/lists/\* \
&& sudo apt --yes install python3.11\
&& sudo apt --yes install python3.11-dev \
&& sudo apt-get install -y python3.11-venv \
&& cd python_yahoo_finance_option_chain \
&& echo "The follow command MUST/SHOULD run as user non root"; \
&& python3.11 -m venv my_project_env \
&& source my_project_env/bin/activate

```

## cleanup apt install  DOESN'T WORK

```bash
#!/bin/bash \
sudo apt-get --yes autoclean \ 
&& sudo apt-get --yes --auto-remove autoremove \
&& sudo apt-get --yes clean  \
&& sudo rm --recursive --force /var/lib/apt/lists/* \ 
&& sudo rm -Rf /usr/share/man \
&& sudo rm --recursive --force /usr/share/doc \
```

## activate venv

```bash
source my_project_env/bin/activate
````

## HIT => leave venv

```bash
# type simple inside shell
deactivate
```

## [FIX issue pip: cannot execute: required file not found](https://askubuntu.com/questions/1480890/pip-disappeared-after-system-upgrade)

```bash
sudo apt update
sudo apt install pipx
pipx ensurepath
pipx completions
pipx upgrade-all

```

## [FIX pip-disappeared-after-system-upgrade ](https://askubuntu.com/questions/1480890/pip-disappeared-after-system-upgrade)

```bash
python3 -m pip install --upgrade pip
```

## install project package

```bash
# pip install yahoo_fin
# or better 
pip3 install yahoo_fin
```



