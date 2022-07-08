# Python

## `requirements.txt`

### `pip freeze` gives local file links rather than version numbers

Currently an open issue with `pip` version 20.1. Use the following workaround:

```
pip list --format=freeze > requirements.txt
```

source: [stackoverflow](https://stackoverflow.com/questions/62885911/pip-freeze-creates-some-weird-path-instead-of-the-package-version)

## Flask


