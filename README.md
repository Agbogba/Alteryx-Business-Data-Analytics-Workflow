
This project covers different Alteryx Designer Workflow in order to respond to Business needs:  

* The file "challenge_120_start_file.yxmd" contains a workflow throught which I determine the most popular names for Males and Females babies that were registered between the years of 1880 and 2017 for each available year.

* The file "challenge_1_start_file.yxmd" contains a workflow throught which I blended two data sets: one conraining Customer Records with a series of postal codes and another containing postcode ranges.

* The file "challenge_2_start_file.yxmd" contains a workflow that prepare delimited data by removing quotes and double quotes. For this I used the following Tools:
  * Text To Columns Tool to separate data by commas into columns, 
  * Formula Tool to strip quotes within columns,
  * DateTime Tool to reformat DateTime data,
  * Select Tool to rename columns, resize data types and choose appropriate columns for the output data,
  * Browse Tool to view the output data

* The file "challenge_38_start_file.yxmd" contains a workflow that blends three sources of data tables named "Product Group", "Region Reference" and "Data" and create a batch output for each product-region combination. For this I used the following Tools:
  * Sample Tool to extract usefull records both in "Region Reference" and "Product Group Reference",
  * Twice the Find and Repalace Tool, first to combine the "Data" table and the "Region Reference" table and secondly to combine the output data with the "Product Group Reference" table,
  * The Formula Tool to create the batch output files names,
  * The Output Data Tool to write the data into (.csv) format       


