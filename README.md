## Creating Virtual Environment with _virtualenv_



1. Open your Terminal/Command prompt :<br><br>

2. From Python 3.3, a subset of virtualenv has been integrated in the Python standard library under the venv module. If you are using Python 2, you can install virtualenv with:
```
pip install --user virtualenv
```
3. Create a virtual environment with :
```
virtualenv myenviro
```
4. For Python >= 3.3 use :
```
python -m venv myenviro
```


5. Go to the 'Scripts' folder in your newly created Environment & RUN :<br>

```
activate
```
6. To deactivate the virtual environment, you can run 
```
deactivate
```



## Adding Virtual Environment to Jupyter Notebook

7. Install ipykernel which provides the IPython kernel for Jupyter : 
```
pip install ipykernel
```

8.  Add your virtual environment to Jupyter by typing:
```
python -m ipykernel install --user --name=myenviro
```

 - This should print the following:
```
Installed kernelspec myenviro in /home/user/.local/share/jupyter/kernels/myenviro
```

9.  Open your Jupyter notebook & check under the _new_ tab

10. Deleting your virtual environment :
- To list existing Jupyter virtual environments
```
jupyter kernelspec list
```
- To remove the environment from Jupyter : 

```
jupyter kernelspec uninstall your_environment_name
```
- Remove your environment folder.