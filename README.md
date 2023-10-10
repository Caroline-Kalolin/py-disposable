# py-disposable
A disposable Python repository for proof of concept and experiments


## Download packages offline
To download the Python offline packages, enter the package name and version in the "requirements.txt" file. 

In command prompt, run this command on the machine that can download these packages online.

```
python -m pip download -r requirements.txt -d ./lib --platform win_amd64 --python-version 310 --no-deps
```

To run on Unix/Linux, run this command.
```
/usr/local/bin/python3 -m pip download -r requirements.txt -d ./lib --platform win_amd64 --python-version 310 --no-deps
```

## Clone repository

**Error: "Unable to resolve "unable to get local issuer certificate" using git on Windows with self-signed certificate"**

In command prompt, run the following command.
```
git config --global http.sslbackend schannel
```

## Install offline packages

In command prompt, run this command to install the Python packages offline.
```
python -m pip install --no-index -f ".\lib" -r ".\requirements.txt"
```