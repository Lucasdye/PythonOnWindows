# PythonOnWindows
Little tutorial to install Python on Windows OS

## Preamble
Installing Python on Windows is not as straight forward as installing it on Linux or Mac Os.
That's why I've created this little tutorial.

## Installation Guide
### Does Python exist on my OS ? 
First you'll have to check if Python is installed on your system by invoking the Python Launcher via a terminal command:
```
py --version
```
Output expected:
```
Python X.X.X
```
If Python isn't installed, download it here:
https://www.python.org/downloads/windows/
Remember to select the custom installation to add the python.exe to the Path environment variable. Sometimes the path of the python.exe isn't
correctly added to the Path environment variable even when specified. If it's the case, please follow the next step.

Secondly, you'll have to check if the python.exe has been correctly added to the Path environment variable. To do so enter the command:
```
python --version
```
If an error message occurs, there's a chance that the python.exe path is lacking in the envrironment variable Path.

### Adding manually python.exe to the environment variable Path
1] To modify Window's environment Path enter in the terminal or Powershell:
```
sysdm.cpl
```
2] Click on 'Environments Variables' located in the Advanced tab.
Under 'System Variables' find 'Path', click on 'Edit' and add the path to the location of the python.exe (usually located in the AppData folder): C:\Users\YourName\AppData\Local\Programs\Python\Python3Xx\
Add also the python script folder:
C:\Users\YourName\AppData\Local\Programs\Python\Python3Xx\Scripts

3] Cick on 'OK', restart the computer, test if python.exe is find by the system by tiping in the terminal (the python version should be displayed):

```
python --version
```
et voilà !








