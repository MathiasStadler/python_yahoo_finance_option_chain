# project path

## test python already installed

```bash
python3 --version
> Python 3.11.2
```

## install python and

``bash
#!/bin/bash \
sudo apt update \
&& sudo apt upgrade \
&& sudo apt-get --yes autoclean \
&& sudo apt-get --yes --auto-remove autoremove \
&& sudo apt-get --yes clean  \
&& sudo rm --recursive --force /var/lib/apt/lists/* \
&& sudo apt --yes install python3.11\
&& sudo apt --yes install python3.11-dev \
&& sudo apt-get install -y python3.11-venv \
&& sudo python3.11 -m venv my_project_env \
&& source my_project_env/bin/activate
```

sudo apt-get update
sudo apt install python3-dev
sudo apt install python3-venv