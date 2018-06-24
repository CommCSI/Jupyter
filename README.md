# Installing Jupyter Notebook on Centos 7

**Make sure you are in root `su` or use `sudo` before each command**

**To make sure repos are there and up-to-date.
```bash
yum install epel-release
yum update
```
Install everything you need for Jupyter Notebook.
```bash
yum -y install gcc gcc-c++ kernel-devel install python-devel libxslt-devel libffi-devel openssl-devel python-pip
```
>**Note:**_There are 2 version errors that might come up._                                                 
>                                                                                                          
>`rtslib-fb 2.1.63 has requirement pyudev>=0.16.1, but you'll have pyudev 0.15 which is incompatible.`     
>`ipapython 4.5.4 has requirement dnspython>=1.15, but you'll have dnspython 1.12.0 which is incompatible.`
>                                                                                                          
>Use to following to resolve errors:                                                                     
>`sudo pip install pyudev==0.16.1`                                                                           
>`sudo pip install dnspython==1.15`     

Install Jupyter.
```bash
pip install jupyter jupyter notebook
```

To check version use:
```bash
python --version && pip --version
```
## Starting Jupyter Notebook
Goto terminal and type the following and you default browser will open up.
```bash
jupyter notebook
```
