# Batch Ingestion Proof of Concept


Document Author: [Caroline Lim](mailto:caroline.lim@apa.com.au)

Updated Date: 10 Oct 2023

---

## Install offline packages
Python offline packages have to be downloaded into PY-Disposable\lib for pip install to work.

Please enter the package name and version in the "requirements.txt" file. Then in command prompt, run this command to install the Python packages offline.

```
.\Scripts\Python.exe -m pip install --no-index -f "..\lib" -r "requirements.txt"
```