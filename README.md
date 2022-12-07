# pylance-import

Steps to reproduce:

1. Install packages

```bash
python -m venv env
source env/bin/activate
cd package-1
pip install -e . --config-settings editable_mode=compat
cd ../package-2
pip install -e . --config-settings editable_mode=compat
```

2. Open VS Code and navigate to package-2/package_2/main.py

3. Try to import the function by pressing `ctrl+.`

### Current Behavior
 
The code action does not list the correct import 

### Expected Behavior

Pylance adds the correct import as option to the code actions.
