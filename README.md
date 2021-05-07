# Information-Architecture-Final

There are several Broad steps used in this process of Setting up this Pipeline. We will be going through them genearlly to ensure that you know what to do and when and how to set this all up in your own enviroment.

IT should be noted that There is a great deal of refrene material in the provided documents. 

Step 1: Set up an AWS account. Please refferene the "IA Donors DW Architecture Final.png" and IA donors_dw Network Diagram V3.pdf documents provided for an overview of the AWS services that will be used. Note: This documentation assumes a certain degree of fammilarity with AWS. We will not be detailing set up of an amazon web service enviroment here.

Step 2: Create an S3 Bucket. 

Step 3: Run the two provided sql scripts in mysql worckbench. Run "createdb_final_V3.sql" first and then "procedures_final_V3.sql"

Step 4: Open Jupyter Notebook and run the two python scripts "Onboard Historical Data Final.ipynb" and "Onboarding Historical Stats Final.ipynb". 
        Important Note: That the scripts can not be run as is. You will need to make small revisions for full functinality in your enviroment. The fields that need         to be changed are:
        
        To connect to mysql you must change the following information in both scripts. 
        -host_name 
        -u_name
        -pwd
        
        To connect to your Jupyter Notebook to AWS you must change the following information in "Onboard Historical Data Final.ipynb" script. 
        -s3pathName 
        -FileNameFullPath
        -filenames3
        
        To connect to your Jupyter Notebook to AWS you must change the following information in "Onboarding Historical Stats Final.ipynb" script. 
        -s3pathName 
        -s3pathName1
        -FileNameFullPath
        -FileNameFullPath1
        -filenames3 
        -filenames3_1
        
The basic set up is all done. You should not run into serious issues. If you do it may be one of the following issues. 

Step 5: Trouble shooting Steps
-Please double check Step 4 to ensure that you made tha appropriate edits to the Python scripts before running them in Jupyter Notebook.
-Please make sure that the S3 bucket you set up is Public.

---

Daily Updates 

Updates will need to be made to the 


