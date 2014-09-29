Python scripts using miralib to perform different batch calculations:

It uses JPython:

https://wiki.python.org/jython/JythonFaq/DistributingJythonScripts

In the jython folder:
* cp jython.jar jythonlib.jar
* zip -r jythonlib.jar Lib
* cp jythonlib.jar ../mirador/tools/scripts/

In the app folder:
* jar ufm jythonlib.jar manifest-miralib.mf

How to run network script:

```bash
 java -jar jythonlib.jar network.py -in diabetes/export/profile-config.mira -out diabetes/network/network.csv
```