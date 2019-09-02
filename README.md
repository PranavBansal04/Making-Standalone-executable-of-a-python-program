# Making-Standalone-executable-of-a-python-program

Steps to be followed:<br /> 
1. Go to your command prompt (Start -> Run -> cmd) and open in administration mode.<br /> 

2. go to the scripts folder inside python.<br /> 

type the following command cd c:\python36\scripts press enter, this should be where your pip.exe file is located.<br /> 
(dont forget to replace your python version in 'python*36*')<br /> 

3.Once you are in this directory type pip install pyinstaller press enter.<br /> 

4. copy the python(.py) file which contains the program to the scripts folder.<br /> 

5.copy your icon logo to the scripts folder as well. The extension of the logo file should be '.ico'. You can convert any file to '.ico' using online tools.<br /> 

6. Run the following command:<br /> 

pyinstaller.exe --onefile --windowed --icon=calc.ico main.py<br /> 

(replace main.py with the name of your file)<br /> 

--If you do not want to provide a icon file then si ply run the following command which will use the default logo:<br /> 
pyinstaller.exe --onefile --windowed main.py<br /> 

Once the execution of this command is completed, a new folder with the name dist will be formed inside scripts folder inside which you will find your stand alone executable file.


#One important thing to note is that the version of the file depends on the system version of your system. If you are using the 64-bit version then the appliction created will also be 64 bit and it will be supported only in 64 bit system. If you want to make a 32-bit version of the same application then you can repeat the aboe process in a 32-bit system.

#Another notable thing is although we are creating a standalone executable yet the resources used by the code still need to b provided explicitly. For example if you are using some images or csv files in your code then these should always be present along with the .exe file. Absence of these files will cause error.
