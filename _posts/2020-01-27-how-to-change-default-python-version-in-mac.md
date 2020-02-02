# How to change the default Python version in Mac

By default, MacOS directs to Python 2. This tutorial is about how to change it to other version of Python (like 3).

Open the terminal.

Change your defulat Python version first  
```
python --version
```

Install python-3 using Homebrew (https://brew.sh).  
```
brew install python
````

Look where it is installed.  
```
ls -l /usr/local/bin/python*
```

The output should look like this:  
```
lrwxr-xr-x  1 keunsoopark  admin  38 Oct  2  2018 /usr/local/bin/python -> ../Cellar/python@2/2.7.15_1/bin/python
lrwxr-xr-x  1 keunsoopark  admin  39 Nov 29 12:27 /usr/local/bin/python-build -> ../Cellar/pyenv/1.2.15/bin/python-build
lrwxr-xr-x  1 keunsoopark  admin  45 Oct  2  2018 /usr/local/bin/python-config -> ../Cellar/python@2/2.7.15_1/bin/python-config
lrwxr-xr-x  1 keunsoopark  admin  39 Oct  2  2018 /usr/local/bin/python2 -> ../Cellar/python@2/2.7.15_1/bin/python2
lrwxr-xr-x  1 keunsoopark  admin  46 Oct  2  2018 /usr/local/bin/python2-config -> ../Cellar/python@2/2.7.15_1/bin/python2-config
lrwxr-xr-x  1 keunsoopark  admin  41 Oct  2  2018 /usr/local/bin/python2.7 -> ../Cellar/python@2/2.7.15_1/bin/python2.7
lrwxr-xr-x  1 keunsoopark  admin  48 Oct  2  2018 /usr/local/bin/python2.7-config -> ../Cellar/python@2/2.7.15_1/bin/python2.7-config
lrwxr-xr-x  1 root         wheel  69 Dec  9 15:31 /usr/local/bin/python3 -> ../../../Library/Frameworks/Python.framework/Versions/3.7/bin/python3
lrwxr-xr-x  1 root         wheel  76 Dec  9 15:31 /usr/local/bin/python3-config -> ../../../Library/Frameworks/Python.framework/Versions/3.7/bin/python3-config
lrwxr-xr-x  1 root         wheel  71 Dec  9 15:31 /usr/local/bin/python3.7 -> ../../../Library/Frameworks/Python.framework/Versions/3.7/bin/python3.7
lrwxr-xr-x  1 root         wheel  78 Dec  9 15:31 /usr/local/bin/python3.7-config -> ../../../Library/Frameworks/Python.framework/Versions/3.7/bin/python3.7-config
lrwxr-xr-x  1 root         wheel  72 Dec  9 15:31 /usr/local/bin/python3.7m -> ../../../Library/Frameworks/Python.framework/Versions/3.7/bin/python3.7m
lrwxr-xr-x  1 root         wheel  79 Dec  9 15:31 /usr/local/bin/python3.7m-config -> ../../../Library/Frameworks/Python.framework/Versions/3.7/bin/python3.7m-config
lrwxr-xr-x  1 keunsoopark  admin  39 Oct  2  2018 /usr/local/bin/pythonw -> ../Cellar/python@2/2.7.15_1/bin/pythonw
lrwxr-xr-x  1 keunsoopark  admin  40 Oct  2  2018 /usr/local/bin/pythonw2 -> ../Cellar/python@2/2.7.15_1/bin/pythonw2
lrwxr-xr-x  1 keunsoopark  admin  42 Oct  2  2018 /usr/local/bin/pythonw2.7 -> ../Cellar/python@2/2.7.15_1/bin/pythonw2.7
```

Change the default Python to the version you want from above  
```
ln -s -f /usr/local/bin/python3.7 /usr/local/bin/python
```

Change if the change was successful  
```
python --version
```