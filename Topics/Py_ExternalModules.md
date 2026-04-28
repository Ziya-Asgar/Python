# External Modules

- [External Modules](#external-modules)
  - [`pip`](#pip)
  - [`uv`](#uv)

---

---

Python has a rich standard library that you can use immediately in your project. In case you need a package that isn’t available in the standard library, you can find it on the Python Package Index (pypi.org).

The Python Package Index (PyPI) is the largest Python repository. It contains many Python packages developed and maintained by the Python community.

---

---

## `pip`

Pip is the package installer for Python. Pip allows you to install packages from PyPI and other repositories.

Python comes with `pip` by default. To check if pip is available on your computer, you can open the command prompt (or Powershell) on Windows and type the following command:

```
pip --version
```

To install a package from PyPI, you use the following command on Windows:

```
pip install <package_name>
```

To install a package with a specific version, you use the following command:

```
pip install <package_name>==<version>
```

To list all installed packages, you use the following pip command:

```
pip list
```

To check what packages are outdated, you use the following command:

```
pip list --outdated
```

To uninstall a package, you use the pip uninstall command:

```
pip uninstall <package_name>
```

To show the dependencies of a package, you use the following command:

```
pip show <package_name>
```

To execute a shell command on a jupyter notebook, we have to use the exclamation mark - `!` - before our code:

```python
!pip install <package_name>
```

---

---

## `uv`

`uv` is a fast Python package and project manager. There are different ways to install `uv`. However, considering that python comes with `pip`, one easy way to install `uv` is to use the below command:

```sh
pip install uv
```

To run a python code (in a `.py` file) with `uv`, we can use the below code:

```sh
uv run file_name.py
```

---

---
