# middleware

In the process, following the tutorial in [Medium](https://medium.com/@naomi.fridman/install-pyspark-to-run-on-jupyter-notebook-on-windows-4ec2009de21f) to install PySPARK, to use local.

There ir neccesary see the environment where packages are installing. In windows with Anaconda it is possible looking in the GUI.

When findpark is already installed, it is necessary to wrhite the path into ```findspark.init()```

```python
import findspark
findspark.init('C:\spark\spark-3.0.0-preview2-bin-hadoop2.7')
```
An exception will appear if I use Anaconda instead Python direcly. Then is necessary to install notebook an not use Anaconda.
```python
Exception: Java gateway process exited before sending the driver its port number
```
After install again the environment from zero. now it appears a new error when import Sklearn. (but Spark it is ok).
```python
ImportError: cannot import name '__check_build' from partially initialized module 'sklearn'
(most likely due to a circular import) (C:\Users\mikes\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\LocalCache\local-packages\Python38\site-packages\sklearn\__init__.py)
```
Apparntly (not 100% sure) it  happens when I install Python from Windows Store, instead directly.
Some tutorials suggest to install the pakage from [diferent source](https://www.lfd.uci.edu/~gohlke/pythonlibs/#scikit-learn). It is necessary install the pakage  according to the version of Python, cp33 means CPython 3.3 ([source](https://stackoverflow.com/questions/28568070/filename-whl-is-not-supported-wheel-on-this-platform))
