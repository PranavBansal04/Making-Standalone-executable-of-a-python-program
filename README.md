# Making-Standalone-executable-of-a-python-program

Steps to be followed:
1. Go to your command prompt (Start -> Run -> cmd) and open in administration mode.
2. go to the scripts folder inside python.
type the following command cd c:\python36\scripts press enter, this should be where your pip.exe file is located.
(dont forget to replace your python version in 'python*36*')
3.Once you are in this directory type pip install pyinstaller press enter.
4. copy the python(.py) file which contains the program to the scripts folder.
5.copy your icon logo to the scripts folder as well. The extension of the logo file should be '.ico'. You can convert any file to '.ico' using online tools.
6. Run the following command:
pyinstaller.exe --onefile --windowed --icon=calc.ico main.py

(replace main.py with the name of your file)

--If you do not want to provide a icon file then si ply run the following command which will use the default logo:
pyinstaller.exe --onefile --windowed main.py
