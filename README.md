# NamasteMart Order Validation System
NamasteMart, an online mart operating in Bangalore and Mumbai, generates daily transaction files that need validation. This project involves creating a system to validate these files and notify the business of any issues.

#### Folder Structure:
NamasteKart\n
incoming_files
success_files
rejected_files

#### Read Files: 
Read all files from the current date folder in incoming_files.

#### Validations:
Product ID must be present in the product master table.
Total sales amount should be the product of the product price and quantity.
Order date should not be in the future.
No field should be empty.
Orders should be from Mumbai or Bangalore only.

#### File Handling:
Files with no issues are moved to success_files.
Files with any validation failures are moved to rejected_files.
For each rejected file, create an error file listing the failed records and reasons for rejection.

#### Email Notification:
Send an email summarizing the validation results, including the number of incoming, successful, and rejected files.

=> This is contains a Python program for daily processing of orders data files and validate the list of orders and detect the errors in the list and then separate the file into 'success' and 'rejected' folders including the 'error_reason' file and then sends the e-mail containing the information of 'total_files', 'success_files' and 'rejected_file'.

This project was given as an assignment in NamasteSQL's Python for Data Analysis(Zero to hero) course.
I have taken inspirations from the winner Vaibhav Desai's submission. Thanks to him and Ankit Bansal sir for the guidance.
I have made improvements in the code as it was not working for different test cases, also I've well defined the code.
Thank you!
