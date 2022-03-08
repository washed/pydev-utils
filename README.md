# pydev-utils

## ufmt_wrapper

### Install

pydev-utils is published on pypi. Use pip to install it:
```bash
pip install pydev_utils[all]
```

### Usage in VSCode

Configure VSCode to use `black` as your formatter and set `Python > Formatting: Black Path`: to
```
pydev_utils.ufmt_wrapper
```

or in `settings.json`:
```json
"python.formatting.blackPath": "pydev_utils.ufmt_wrapper"
```

Now you can use the regular `Format Document` commands from the command pallette. Files will be auto-formatting and imports sorted and grouped.
It will not remove duplicate imports.

**NOTE:** ufmt only works on saved files and will not format unsaved changes in your editor.
