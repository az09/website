# website
gis-lab.info


# dev
```
$ git clone https://github.com/gis-lab-info/website.git
$ cd website
```

There are 2 ways to run the development server:


```
$ python -m http.server
```

or with includes and everything

## Linux:
First time
```
$ sudo apt install php-cgi php-xml python3-virtualenv (?)
$ virtualenv -p python2 env
$ source env/bin/activate
$ pip install bottle eventlet
$ ./ssi-server --skip-missing
```
To-Do: Switch to Python3

Second start (when environment is not activated)
```
$ source env/bin/activate
$ ./ssi-server --skip-missing
```
## Windows (cmd):

[Download](https://windows.php.net/download/) and unpack PHP into `c:\tools\php` for example.

```
set path=%path%;c:\tools\php
c:\Python39\Scripts\pip install virtualenv
c:\Python39\Scripts\virtualenv.exe -p python2 env
env\Scripts\activate
pip install bottle eventlet
python ssi-server --skip-missing
```