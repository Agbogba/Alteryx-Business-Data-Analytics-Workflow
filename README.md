
This project presents my solutions where I built Alteryx Designer Workflow with Business data to address ADAPT program challenges.


1. Challenge #120: Popular Baby Names:
 
The file "challenge_120_start_file.yxmd" contains a workflow throught which I determine the most popular names for Males and Females babies that were registered between the years of 1880 and 2017 for each available year included in the file "names.yxdb". For this I used the following Tools:

    * a Text to Columns Tool to split string data to Columns,
    * a Formula Tool to retrieve substring withing a column,
    * a Select Tool to remame Field Columns and choose relevant Fields,
    * a Filter Tool to filter the data by Gender value "F",
    * 2 opposite Select Tool to rename the Field and choose relevant Fields for each opposite data,
    * 2 opposite Summarize Tool to group each data by year and taking the other values
    * a Join Tool to join the data on year values and,
    * a Browse Tool to view the data J          


2. Challenge #1: Join to Range:

The file "challenge_1_start_file.yxmd" contains a workflow throught which I blended two data sets: one conraining Customer Records with a series of postal codes and another containing postcode ranges. For this I used the following Tools:

    * a Text to columns Tool to split string data to columns by dash,
    * a Select Tool to format splited string data to integer,
    * an Append Fields Tool to join both the input data files,
    * a Filter Tool to filter the data by the Field named Postal Area,
    * a Summarize Tool to group the data by Fields named "Region", "Sales Rep" and "Responder" and count Filed named "Customer ID"      


3. Challenge #2: Preparing Delimited Data:

The file "challenge_2_start_file.yxmd" contains a workflow that prepare delimited data by removing quotes and double quotes from an input data. For this I used the following Tools:

    * a Text To Columns Tool to separate data by commas into columns, 
    * a Formula Tool to strip quotes within columns,
    * a DateTime Tool to reformat DateTime data,
    * a Select Tool to rename columns, resize data types and choose relevant columns for the output data,
    * a Browse Tool to view the output data
 

4. Challenge #38: Data Blending for Batch Output:

The file "challenge_38_start_file.yxmd" contains a workflow that blends three sources of data tables named "Product Group", "Region Reference" and "Data" and create a batch output for each product-region combination. For this I used the following Tools:

    * a Sample Tool to extract usefull records both in "Region Reference" and "Product Group Reference",
    * a Find and Repalace Tool to combine the "Data" table and the "Region Reference" table,
    * a Find and Repalace Tool to combine the previous output data with the "Product Group Reference" table
    * a Formula Tool to create the batch output files names,
    * an Output Data Tool to produce 15 output files, one for each product-region combination into (.csv) format to a directory named "Challenge38-files".
    
5. Challenge #35: Data Cleansing Practice

The file "challenge_35_start_file.yxmd" contains 4 independant workflows that perform data cleansing:

    * The first workflow hepls removing leading zeroes using one Fornula Tool to trim zeros on left side followed by a Filter Tool to change the type of string values to integer and a Browse Tool
    * The second workflow helps to trim leading zeroes and/or descriptive text at the end by using one Record ID Tool to enumerate the records followed by one Formula Tool to remove zeroes on left if applicable, a Filter Tool to select and rename appropiate fileds and a Browse Tool
    * The third workflow uses a Formula Tool followed by a Select Tool amd a Browse Tool to remove the ID if the data value ends with ID
    * The fourth workflow uses a Formula Tool followed by a Select Tool and Browse Tool to remove anything after 8 if more than 8 chars, and add “SC” to the front if only 6.

6. Challenge #46: Formatting a Date from an Integer

The file "challenge_46_start_file.yxmd" contains a workflow with one Formula Tool followed by a DateTime Tool and a Select Tool to solve the following issue:

    Use case: The Input contains dates formatted as year, month and day. In this case, the first character determines if the year should begin with 19 or 20. If the first character is 0 then the year starts with 19, and when the first character is 1 the year starts with 20. The remainder of the date following the 0 or 1 is the remaining year digits followed by month followed by day.
    Objective: Please convert these strings into date formatted field.
    


