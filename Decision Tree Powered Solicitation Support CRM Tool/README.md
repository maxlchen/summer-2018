## Solicitation Support CRM Tool

This application is meant to automate the task of testing whether or not a company in the solitication initiation list is already in the CRM. 
This method uses a Fuzzy Matching (approximate string matching) and a Supervised Machine Learning classifier to decide whether or not a company is included in the CRM already.

## Required Packages

The following program must be installed:

<a href="https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2017">Microsoft Visual C++ Build Tools (Click Me)</a>

Python 3 *must* be installed. Furthermore, during installation, the <b><u>"local environment"</u></b> *must* be checked off in order to allow the program to access Python by simply running "python."
Ideally, use the <a href = "https://www.anaconda.com/download/#download">Anaconda Distribution of Python (Click Me)</a> to simplify things. I cannot stress the importance  of checking off using <b><u>"local environment"</u></b>.

To see what I mean by checking off the local environment, please see the image at the bottom of this page.

The following packages must be installed:

pickle (Should come installed)

	python -m pip install pickle

pandas (Ignore if using Anaconda)
	
	python -m pip install pandas

sklearn (Ignore if using Anaconda)

	python -m pip install sklearn

tkinter (Should come installed)

	python -m pip install tkinter

openpyxl (Ignore if using Anaconda)

	python -m pip install openpyxl

Pillow (Ignore if using Anaconda)
 
	python -m pip install pillow

fuzzyset

	python -m pip install fuzzyset

fuzzywuzzy

	python -m pip install fuzzywuzzy

fuzzywuzzy - Levenshtein

	python -m pip install fuzzywuzzy[speedup]




## **How to Use This App**

1. EXTREMELY IMPORTANT: follow the instructions above. Without <strong>all</strong> of the libaries, this script will not compile.
2. <strong>Make sure that the most recently trained classifier is in the same folder!</strong> This file is, and should be, named "decisiontree.sav"
3. Make sure you have the most recent CRM <u>appropriate for the Solicitation File being used</u>.
4. Make sure the following data is formatted to meet the following: First solicitation entry begins at row 28, Company Name begins in Column C, Contact Email begins in Column F, Country begins in Column H.
5. Launch the application and follow the instructions listed.

## Limitations

The format of the Solicitation Support Template keeps changing. The data always begins at row 28. At the moment, it seems most common that "Company Name" will be in Column C, "Contact Email" will be in Column F, and "Country" will be in Column H. If this is not the case, please format the data so that it will satisfy these conditions.
These discrepancies may occur due to differing templates (e.g. "Contact Name" taking one column as opposed to "Contact First Name" and "Contact Last Name" taking two columns).
	Potential Improvement: Select the rows by name, instead of column letter. The current issue is that rows 1-27 are formatting intended for the client, and the currently used excel reader does not permit name selection.

The model does not differentiate between "No match" and "Company match, but new contact needed." This is due to Decision Trees holding much higher accuracy on two outcomes, as opposed to three, because of the use of Gini Impurity as opposed to Entropy.

This also comes down to what the data represents. The idea is that either way, the analyst will have to create a new entry in the CRM, regardless of whether it is "No match" or "Company match, but new contact needed."


## Metrics

In creating a model for this application, a Decision Tree and a Logistic Regression were tested.

Decision Tree mean accuracy score: 0.9621

Logistic Regression mean accuracy score: 0.7273

## Adding Anaconda to PATH
![Screenshot](https://github.com/maxlchen/summer-2018/blob/master/Decision%20Tree%20Powered%20Solicitation%20Support%20CRM%20Tool/image/AnacondaInstall.png)

## Appearance

As of <i>August 1, 2018</i>
![Screenshot](https://github.com/maxlchen/summer-2018/blob/master/Decision%20Tree%20Powered%20Solicitation%20Support%20CRM%20Tool/image/gui-screenshot.png)

*Developer:*<br/>
*Max Chen (Cornell University '21)*








