# middleware

In the process, following the tutorial in [Medium](https://medium.com/@naomi.fridman/install-pyspark-to-run-on-jupyter-notebook-on-windows-4ec2009de21f) to install PySPARK, to use local.

There ir neccesary see the environment where packages are installing. In windows with Anaconda it is possible looking in the GUI.

When findpark is already installed, it is necessary to wrhite the path into findsspark.init()

```python
import findspark
findspark.init('C:\spark\spark-3.0.0-preview2-bin-hadoop2.7')
```
