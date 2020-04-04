# django-draft
useful django options - for Linux Ubuntu

1. virtualenv is liklely the most flexible / classic Envoronment Manager for Python Projects
2. To create Virtual Environment from Python version not installed on your system, it should first be downloaded/compiled and configuered.
--- download required python source from https://www.python.org/downloads/
--- extract the downloaded/compressed tar archive via command like: tar -xvzf Python-3.x.yz.tgz
--- configure the future python installation: 
    cd Python-3.x.yz.tgz
    ./configure prefix=/home/user/alternate_python
    ./make
    ./make altinstall # the new version of python executable(s) will be put into /home/user/alternate_python/bin folder
--- run creation of new environment via command like: virtualenv --python=/home/user/alternate_python/bin/python3.x /home/use/newenvironment
--- activate new environment: cd /home/use/newenvironment
                              source bin/activate
--- the command prompt will change accordingly
--- deactivate when requried via command: deactivate

p.s. sometime the system requries installing zlib library for correct compiling of python packages:
sudo apt install zlib1g-dev
