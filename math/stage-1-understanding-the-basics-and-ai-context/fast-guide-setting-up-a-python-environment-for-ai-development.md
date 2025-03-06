---
description: >-
  This guide will assume that you know basics of software development, so you
  already have linux based system or MacOS based system. If you don't, get one!
icon: python
---

# Fast Guide: Setting Up a Python Environment for AI Development

## 1. Install Python

First, ensure you have Python installed (recommended version: **3.10+**).

```sh
➜  ~ python --version               
Python 3.12.9
➜  ~ 
```

**If not installed, download it:**

{% embed url="https://www.python.org/downloads/" %}

Use the installer and make sure to check **"Add Python to PATH"**.



## **2. Set Up a Virtual Environment (Recommended)**

A virtual environment keeps dependencies isolated per project.

```sh
➜  ~ python -m venv trysoft_learn_ai
```

Activate it:

```sh
➜  ~ source trysoft_learn_ai/bin/activate
(trysoft_learn_ai) ➜  ~ 
```

To deactivate:

```
(trysoft_learn_ai) ➜  ~ deactivate        
➜  ~ 
```



## 3. Install Essential Libraries

Inside your virtual environment, install core AI packages:

```sh
(trysoft_learn_ai) ➜  ~ pip install numpy scipy pandas matplotlib seaborn jupyter scikit-learn
```

For deep learning:

```sh
(trysoft_learn_ai) ➜  ~ pip install tensorflow torch torchvision torchaudio
```



## **4. Set Up Jupyter Notebook (Optional, but Useful for AI Workflows)**

```sh
(trysoft_learn_ai) ➜  ~ pip install notebook
```

```sh
(trysoft_learn_ai) ➜  ~ jupyter notebook
```

This will launch Jupyter in your browser.



## **5. (Optional) Use Conda for Environment Management**

There is lot of different envs for Python like Conda, venv, pyenv, virtualenv, Poetry, Docker. I don't have any preference for now, so I will be using a default one (venv).



## 6. Set Up an IDE (Recommended: VS Code or PyCharm)

* **VS Code:** Install [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python).
* **PyCharm:** Comes with built-in support for virtual environments.



## 7. First Test – Run a Simple AI Script

Create a file `test.py` and add:

```python
import numpy as np

A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])
print("Matrix multiplication result:\n", np.dot(A, B))

```

Run it:

```sh
python test.py
```

You're Ready to Code AI in Python! 🚀
