# Batch Ingestion Proof of Concept


Document Author: [Caroline Lim](mailto:caroline.lim@apa.com.au)

Updated Date: 10 Oct 2023

---

## Install offline packages on virtual environment
Python offline packages have to be downloaded into PY-Disposable\lib for pip install to work.

- Change directory to the virtual environment folder path.
- Create the "requirements.txt" file in the virtual environment folder.
- Enter the packages required for installation in the "requirements.txt". 
- In command prompt, run this command to install the Python packages offline.

```
.\Scripts\Python.exe -m pip install --no-index -f "..\lib" -r "requirements.txt"
```