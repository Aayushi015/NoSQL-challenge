**📊NoSQL Database Analysis**

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**📝 Overview**

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
This project analyzes food hygiene ratings across the United Kingdom using MongoDB as a NoSQL database. The data comes from the UK Food Standards Agency, which inspects and rates establishments on hygiene, structural compliance, and confidence in management.

The project was developed to assist the editorial team at Eat Safe, Love, a food magazine, to identify high-performing and underperforming establishments for future articles and reviews.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**📂 Project Structure**

The project is divided into three main parts:

**1️⃣ Database Setup**

-Imported data from establishments.json into a MongoDB database.

-Created a new database named uk_food.

-Populated a collection called establishments.

-Verified the data import using find_one() and listed all collections and databases.

**2️⃣ Data Updates & Cleaning**

-Added a new restaurant in Greenwich (Penang Flavours) to the dataset.

-Retrieved the correct BusinessTypeID for the new restaurant and updated its record.

-Removed all establishments located in the Dover Local Authority.

-Converted fields like latitude, longitude, and RatingValue from strings to proper numeric types to ensure accurate analysis.

**3️⃣ Exploratory Analysis**

-Answered specific data queries requested by Eat Safe, Love editors:

-Establishments with a hygiene score of 20.

-Establishments in London with a RatingValue >= 4.

-Top 5 establishments with RatingValue = 5, sorted by lowest hygiene score and nearest to Penang Flavours.

-Count of establishments in each Local Authority area with a hygiene score of 0, ranked from highest to lowest.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧰 Technologies Used**

Python

MongoDB

Pandas

Jupyter Notebook

PyMongo

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**⚙️ Setup Instructions**

1. Install Required Packages
   
  pip install pymongo pandas
  
3. Import Data into MongoDB
   
   mongoimport --db uk_food --collection establishments --file establishments.json --jsonArray
   
5. Run the Jupyter Notebooks
   
   NoSQL_setup_Yoshi.ipynb - for database setup and modifications.
   
   NoSQL_analysis_Yoshi.ipynb - for data analysis and answering editorial questions.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
