## Solicitation Support CRM Tool

This application is meant to automate the task of testing whether or not a company in the solitication initiation list is already in the CRM. 
This method uses a Fuzzy Matching (approximate string matching) and a Supervised Machine Learning classifier to decide whether or not a company is included in the CRM already.

##Required Packages

The following program must be installed:

<a href="https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2017">Microsoft Visual C++ Build Tools (Click Me)</a>

Python 3 *must* be installed. Furthermore, during installation, the "local environment" *must* be checked off in order to allow the program to access Python by simply running "python."

The following packages must be installed:

pickle

	python -m pip install pickle

pandas
	
	python -m pip install pandas

sklearn

	python -m pip install sklearn

tkinter

	python -m pip install tkinter

openpyxl

	python -m pip install openpyxl

Pillow

	python -m pip install pillow

fuzzyset

	python -m pip install fuzzyset



##**How to Use This App**

1. EXTREMELY IMPORTANT: follow the instructions above.
2. <strong>Make sure that the most recently trained classifier is in the same folder!!</strong> This file is named "decisiontree.sav"
3. Make sure you have the most recent CRM appropriate for the Solicitation File being used.
4. Launch the application and follow the instructions listed.

*Developers:*<br/>
*Max Chen (Cornell University '21)*








