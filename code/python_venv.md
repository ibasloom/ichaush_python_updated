## Setting Up Python Environment

This guide explains how to set up a virtual environment for your Python project using `pip`. 

**1. Check Python Installation:**

Open a terminal and type `python3`. If Python 3 is installed, you'll see the version information. Otherwise, you'll need to install it.



**2. Create Project Directory:**

Create a directory for your project:

```
mkdir my_project_yt
```
```
cd my_project_yt
```



**3. Create Virtual Environment:**

Create a virtual environment named imran_env_new using venv:


```
python3 -m venv imran_env_new
```



***4. Activate Virtual Environment:***

Activate the virtual environment to use its isolated packages:


```
source imran_env_new/bin/activate
```



***5. Verify Packages (Optional):***

(Optional) You can check the initially installed packages in the virtual environment:

```
python -m pip freeze
```


***6. Install Packages:***

Replace package_name with the actual package you want to install:

```
pip install package_name
```

Example: Install Jupyter Notebook:

```
pip install jupyter
```


```
jupyter notebook
```


***7. Deactivate Virtual Environment:***

When you're done working on your project, deactivate the environment:


```
deactivate
```


