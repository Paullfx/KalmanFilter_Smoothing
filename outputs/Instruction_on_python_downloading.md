# how to update python packages

Step 1:

Go to Python official website: https://www.python.org/downloads/windows/
And download the "Windows installer (64-bit)" for the version that you want

Step 2:

Open the "Windows installer (64-bit)"
And change the following to be different from the default

    a. Uncheck "install for all users" option.
    b. Go for the custom installation.
    c. On next screen specify the directory path for which your user have full access on the computer. (Recommend you to create a file directly under desk C: called e.g. "python39")
    d. Uncheck "create shortcuts for installed application" option.
    e. Make sure "Add python to environment variable" option is Unchecked .
    
now you have downloaded the desired version of python in a file in the local desk C:
(You can have a look at https://stackoverflow.com/questions/33876657/how-to-install-python-any-version-in-windows-when-youve-no-admin-privileges if something goes wrong as you follow the above instructions.)

Step 3: Set the new version of python in the vs code

    a. create a new folder under local desk C:
    b. create a new file in the new folder
    c. select language "python" (Similarly in the BMW internal wiki: https://atc.bmwgroup.net/confluence/pages/viewpage.action?pageId=2006936156)
    d. press "Shift"+"Ctrl"+"P" and  type in 'Python Select Interpreter', then press Enter
    e. click "enter interpreter path" and browse to the python.exe file in the folder that you just downloaded python
    f. now you will see the new python version appearing in the bottom right corner of VS Code

Step 4: Now you can install the needed packages. Remember to add "--proxy 192.109.190.88:8080" when you install anything

use the force:

    C:\py39\python -m pip install numpy --proxy 192.109.190.88:8080 