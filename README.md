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
```shell
$ sudo apt install php-cgi php-xml
$ sudo apt install python3-virtualenv python2-pip-whl python2-setuptools-whl
$ virtualenv -p python2 env
$ source env/bin/activate
$ pip install bottle eventlet
$ ./ssi-server --skip-missing
```

Second start (when environment is not activated)
```
$ source env/bin/activate
$ ./ssi-server --skip-missing
```
## Windows (cmd):

[Download](https://windows.php.net/download/) and unpack PHP into `c:\tools\php` for example.

```shell
set path=%path%;c:\tools\php
c:\Python39\Scripts\pip install virtualenv
c:\Python39\Scripts\virtualenv.exe -p python2 env
env\Scripts\activate
pip install bottle eventlet
python ssi-server --skip-missing
```