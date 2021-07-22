
This project presents my solutions where I built Alteryx Designer Workflow with Business data to address ADAPT Program challenges.


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


