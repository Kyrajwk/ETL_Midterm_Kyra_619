ETL Midterm Project – DSA2040A
1. Project Overview

	This project is a simple ETL (Extract, Transform, Load) pipeline built for the mid-semester exam.
	The goal was to take raw and incremental order data, clean it up, apply useful transformations, 
	and load it into a structured format. Everything is organized into notebooks so it’s easy to 
	follow each step from start to finish.

2. ETL Phases

	(i) etl_extract.ipynb
		In this notebook, I loaded both raw_data.csv and incremental_data.csv, displayed previews of the data, 
		and made basic observations. I looked for missing values, duplicates, and checked the overall structure 
		of each file.

	(ii) etl_transform.ipynb
		Here, I applied six meaningful transformations to both datasets. These included removing duplicates, 
		filling in missing names, dropping rows that couldn’t be used, creating a new column for total price, 
		converting order dates to proper datetime format, and grouping total prices into tiers. Each 
		transformation included a before-and-after look and a short explanation of why it was done.

	(iii) etl_load.ipynb
		Finally, I loaded the transformed datasets into SQLite databases. Both the full and incremental datasets 
		were saved as .db files in the loaded/ folder. I also ran a quick SQL query to confirm that the data was 
		inserted correctly.

3. Tools Used
	i) Python

	ii) Pandas

	iii) SQLite (via sqlite3)

	iv) Jupyter Notebook

	v) VS Code (for development)

4. How to Run the Project

   	(i) Clone or download this repository

	(ii) Make sure you have Python installed (3.8 or above is recommended)

	(iii) Open the project folder in VS Code (or any IDE you prefer)

	(iv) Run the three notebooks in this order:

			- etl_extract.ipynb

			- etl_transform.ipynb

			- etl_load.ipynb

	(v) Transformed files will be saved in the transformed/ folder

	(vi) The SQLite databases will appear in the loaded/ folder

	(vii) You can view the .db files using DB Browser for SQLite or the query cells in the notebook

