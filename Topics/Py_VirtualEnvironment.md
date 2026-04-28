# Virtual Environments

- [Virtual Environments](#virtual-environments)
  - [Creating a virtual environment](#creating-a-virtual-environment)
  - [Activating and deactivating a virtual environment](#activating-and-deactivating-a-virtual-environment)
  - [requirements.txt file](#requirementstxt-file)

---

---

A virtual environment is a self-contained location that enables to maintain a separate and isolated environments for python projects. It helps to manage dependencies, versions, and packages without conflicts accross different projects.

A virtual environment is also a separate directory. So, when we create one, it is recommended to be in folder where a specific python project is.

---

---

## Creating a virtual environment

This is how we can create one on a windows machine:

```sh
python -m venv env_name
```

---

---

## Activating and deactivating a virtual environment

After this command, a directory named **env_name** will be created. To activate the environment, we need to run the code below on windows:

```sh
source env_name/Scripts/activate
```

If the above doesn't work, we can try:

```sh
source env_name/Scripts/activate.bat
```

To deactivate, we run `deactivate`.

---

---

## requirements.txt file

To share the project with others, it's recommended to create a file named `requirements.txt` and the save dependencies to that file. This way we can avoid pushing the whole environment to Git. To create the `requirements.txt` file with all the dependencies, we can use the below code:

```sh
pip freeze > requirements.txt
```

`pip freeze` is a shell command to list all the python libraries and versions. `>` is an operator that pipes the output of `pip freeeze` to the `requirements.txt` file.

After this step, another person can activate a different environment on their end and use this `requirements.txt` file to install all the dependencies. The code that is needed is below:

```sh
pip install -r requirements.txt
```

`-r` stands for installing from a file.

---

---
