# Big-Data-ETL
Extract two Amazon customer review datasets, transform each dataset into four DataFrames, and load the DataFrames into an RDS instance.

## Background
In this assignment, you will put your ETL skills to the test. Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. Your first goal will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

Extract two Amazon customer review datasets, transform each dataset into four DataFrames, and load the DataFrames into an RDS instance.

## Before You Begin
* Create a new repository for this project called "Big-Data-ETL". Do not add this homework to an existing repository.

* Clone the new repository to your computer.

* Inside your local Git repository, create two folders, "part-1" and "part-2", corresponding to the two parts. If you are not planning on doing "part-2" then create the "part-1" folder only.

## Instructions
* Upload the part_one_starter_code.ipynb into Google Colab and create a duplicate of this file.

* Explore the Amazon ReviewsLinks to an external site. datasets and pick two datasets to perform ETL.

* Rename each part_one_starter_code.ipynb file according to the dataset you are using. For example, if you are going to use the Video Game reviewsLinks to an external site. file, rename file, part_one_video_games.ipynb. Repeat the process for the duplicate file you created in Step 2.

* Extract the Data

* Read in each dataset using the correct header and sep parameters.

* Get the number of rows in the dataset.

* Transform the Data

* For each dataset use the schema.sql file located in the Resources folder of the Starter_Code.zip file to create the four DataFrames as follows:

Create the "review_id_df" DataFrame with the appropriate columns and data types.

Create the "products_df" DataFrame that drops the duplicates in the "product_id" and "product_title columns.

Create the "customers_df" DataFrame that groups the data on the "customer_id" by the number of times a customer reviewed a product.

Create the "vine_df" DataFrame that has the "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns.

* Load the Data into an RDS Instance

* Export each DataFrame into the RDS instance to create four tables for each dataset.

NOTE
This process can take up to 10 minutes for each. Ensure that everything is correct before uploading.

IMPORTANT
Do not clear the outputs of your .ipynb files, and do not upload notebooks that contain your RDS password and endpoint. Delete these two items before making your notebook public!

Ensure your repository has regular commits and a thorough README.md file to explain the ETL project.

NOTE
You are allowed to miss up to two Challenge assignments and still earn your certificate. If you complete all Challenge assignments, your lowest two grades will be dropped. If you wish to skip this assignment, click Next, and move on to the next Module.

Comments are disabled for graded submissions in BootCamp Spot. If you have questions about your feedback, please notify your instructional staff or your Student Success Manager. If you would like to resubmit your work for an additional review, you can use the Resubmit Assignment button to upload new links. You may resubmit up to three times for a total of four submissions.

## References
Amazon Customer Reviews Dataset. (n.d.). Retrieved April 08, 2021, from: https://s3.amazonaws.com/amazon-reviews-pds/readme.htmlLinks to an external site.
