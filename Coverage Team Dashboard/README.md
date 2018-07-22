## Coverage Team Live Metrics Dashboard

This application is meant to automate the task of calculating and documenting the statistics of the Coverage team's capabilities. 
As of July 20, 2018, total runtime has been cut to 4.70 seconds on an i5-4570T CPU and 16GB of RAM.

## Required Packages

Python 3 *must* be installed. Furthermore, during installation, the "local environment" *must* be checked off in order to allow the program to access Python by simply running "python."

The following packages must be installed:

datetime

	python -m pip install datetime

pandas
	
	python -m pip install pandas

xlsxwriter

	python -m pip install xlsxwriter

tkinter

	python -m pip install tkinter

openpyxl

	python -m pip install openpyxl

Pillow

	python -m pip install pillow



## **To-Do List:**

1. Include more use cases errors
2. Button to present user with all companies available in the Workbook loaded.
3. Scrollbar
4. Automatically adjusting sizes for text box, logo, buttons


## **Current User-Accessible Functionalities:**

1. Read an Excel Workbook (including individual sheets)
2. Automatically calculate all Live Metrics
3. Write updates to an Excel Workbook, given that it already exists.
4. Save changes to an Excel Workbook
5. Easy-to-read GUI


## **Technical Improvements**

1. Runtime has been cut drastically, from 2+ minutes to 4.70 seconds. This was done by improving the organization of individual script files and implementing more efficient data structures.
2. Memory usage has been cut drastically, from requiring 2GB+ to a negligible amount. This was done by combining the merits of OpenPyxl, Pandas and ExcelWriter. As a result, data is now stored minimally.
3. Users are now aware of the status of their tasks.
4. Many, *but not all* possible errors in usage have been accounted for; these errors will instead result in the text box presenting a possible explanation for the error.


## **Most Important Limitations**
1. Creation of Company objects is *very* dependent on the indices of the Excel Workbook. This application was created specifically for the purpose of updating the Coverage team Live Metrics, which had a very specific workflow.
2. The current method of writing to Excel is dependent on the existence of a file called "Live Metrics Book.xlsx" in the same folder. This can be easily updated by including another filepath prompt, but it has not yet been done so due to the fact that runtime is a bigger concern in this use case.

*Developers:*<br/>
*Max Chen (Cornell University '21)*


## GUI Appearance Documentation

*July 20, 2018*
Omitted








