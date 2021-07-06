# textractor
Textractor reads images and scans (pdf) and extract informations from it such as text, tables and forms.

Most of the code comes from Textractor help section on AWS, but I had to clean it and adapt it to my needs.

How to use it;
0) clone the code somewhere
1) in the same folder create a folder containing your docs OR create an AWS bucket with your files (.jpg and .pdf only)
2) open a terminal and run one of the following commands

- python3 textractor.py --documents mydoc.jpg --text --forms --tables --region us-east-1
- python3 textractor.py --documents ./myfolder/ --text --forms --tables
- python3 textractor.py --documents s3://mybucket/mydoc.pdf --text --forms --tables
- python3 textractor.py --documents s3://mybucket/ --text --forms --tables

Note: if you want only "text" data, just add --text and so on...
