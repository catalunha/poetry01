Tutorial

https://www.youtube.com/watch?v=_XszPRFHQQ4

# Instalando poetry
catalunha@pop-os:~$ curl -sSL https://install.python-poetry.org | python3 -

# Config .bashrc
catalunha@pop-os:~$ nano .bashrc
Add `export PATH="/home/catalunha/.local/bin:$PATH"` to your shell configuration file.
catalunha@pop-os:~$ source .bashrc 

# Criando projeto poetry
catalunha@pop-os:~/apps/python$ poetry new poetry01

abrindo no vscode
catalunha@pop-os:~/apps/python/poetry01$ code .

# Criando e ativando virtual env para este projeto
catalunha@pop-os:~/apps/python/poetry01$ which python
/usr/bin/python

catalunha@pop-os:~/apps/python/poetry01$ poetry env use 3.10
Creating virtualenv poetry01-MElvCAWb-py3.10 in /home/catalunha/.cache/pypoetry/virtualenvs
Using virtualenv: /home/catalunha/.cache/pypoetry/virtualenvs/poetry01-MElvCAWb-py3.10
catalunha@pop-os:~/apps/python/poetry01$ 

catalunha@pop-os:~/apps/python/poetry01$ poetry shell
Spawning shell within /home/catalunha/.cache/pypoetry/virtualenvs/poetry01-MElvCAWb-py3.10
catalunha@pop-os:~/apps/python/poetry01$ . /home/catalunha/.cache/pypoetry/virtualenvs/poetry01-MElvCAWb-py3.10/bin/activate
(poetry01-py3.10) catalunha@pop-os:~/apps/python/poetry01$ 

# Instaland django com poetry

(poetry01-py3.10) catalunha@pop-os:~/apps/python/poetry01$ poetry add django

(poetry01-py3.10) catalunha@pop-os:~/apps/python/poetry01$ poetry add djangorestframework


# Iniciando um projeto django

(poetry01-py3.10) catalunha@pop-os:~/apps/python/poetry01$ poetry run django-admin startproject project .