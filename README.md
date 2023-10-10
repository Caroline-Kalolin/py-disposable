# py-disposable
A disposable Python repository for proof of concept and experiments

❗️ **Works on Windows 64 bit and Python version 3.10.8**

---

## Download packages offline
To download the Python offline packages, enter the packages required in the "requirements.txt" file. 

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

## To create Python virtual environment
Amend the folder path in the command before running it.
```
python -m venv ".\folder-path"
```

## Install offline packages on virtual environment
Python offline packages have to be downloaded into PY-Disposable\lib for pip install to work.

- Change directory to the virtual environment folder path.
- Create the "requirements.txt" file in the virtual environment folder.
- Enter the packages required for installation in the "requirements.txt". 
- In command prompt, run this command to install the Python packages offline.

```
.\Scripts\Python.exe -m pip install --no-index -f "..\lib" -r "requirements.txt"
```