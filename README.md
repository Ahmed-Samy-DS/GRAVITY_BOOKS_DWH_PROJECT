
The goal of this project was to create a robust data warehouse design for loading data from a giant bookstore database. The design includes applying incremental loads to retrieve only the newly added or updated data in the source. Additionally, a brief dashboard was created in Power BI to summarize the running business of the bookstore.

I used the following tools and technologies in this project:

MS SQL Server
SQL
SSIS
SSAS
Excel
Power BI
I also applied slowly changing dimensions Type 1 and Type 2 in many cases as the business required.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
This project is an end-to-end Business Intelligence solution, starting from designing the data warehouse based on the business needs:

First:
I chose the galaxy schema as it was the most suitable approach for this case.

Second:
I created mapping sheets for each dimension and fact table to clarify the source and destination and to show if there were any lookups.

Third:
I started creating ETL packages in SSIS, applying Slowly Changing Dimension Types 0, 1, and 2 in different cases as needed by the business. I handled the incremental refresh in fact tables and created an accumulating fact table for the status to show the entire order life cycle, from order placement to delivery or cancellation.

Fourth:
I used SSAS to gain insights from the data warehouse after loading the data.

Finally:
I created a dynamic Power BI dashboard to provide more detailed insights into our business.
