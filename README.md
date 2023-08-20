# Web Scrapping
### Project description:
Analysis of the UK Food Standards Agency, in particular food hygiene ratings using NoSQL and Bash. Importing the json data using Bash and using NoSQL to perform CRUD operations on the json data as well as exploritory analysis to answer the following questions: 
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
To answer the above questions the following methods were used: 
* Using "$regex" to find specific expressions in the dataset.
* Aggregating & Filtering the data using various methods from MongoDB. 
* Creating a query pipeline to answer the 4th question using the aggregate method. 

#### NOTE:
* > (A) The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the worse the establishment is in these areas.
* > (B) RatingValue refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the better the rating.
*   > > (B.1) This field also includes non-numeric values such as 'Pass', where 'Pass' means that the establishment passed their inspection but isn't given a number rating. We will coerce non-numeric values to nulls during the database setup before converting ratings to integers.

### Libraries used: 
1. pymongo
2. pprint
3. Pandas

#### Folder structure
``` yml
.
├── nosql-challenge
│   ├── Starter_Code    
│   |   ├── NoSQL_analysis_starter.ipynb
│   |   ├── NoSQL_setup_starter.ipynb
│   |   ├── Resources   
│   |   |   ├── establishments.json                                       
|___.gitignore               
|___README.md
``` 


