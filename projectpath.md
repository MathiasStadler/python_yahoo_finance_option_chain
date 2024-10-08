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
&& sudo python3.11 -m venv my_project_env \
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

## leave venv

```bash
# type simple inside shell
deactivate
```

## install project package

```bash
pip install yahoo_fin
# or
pip3 install yahoo_fin
```

pip3 install yahoo_fin