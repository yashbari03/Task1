#1.Loaded the Dataset
I started by loading the Netflix data from a CSV file into a pandas DataFrame so I can work with it in Python.

#2.Handled Missing Values
I checked for any empty or missing data using .isnull(). Instead of leaving them blank, I replaced missing values with "Unknown" so our data remains complete and easier to work with.

#3.Removed Duplicate Rows
Sometimes data is repeated by mistake. I used .drop_duplicates() to keep only unique rows and avoid redundancy.

#4.Standardized Text Values
Text entries like country names or types (e.g., “Movie”, “TV Show”) might be written in different formats. I cleaned them up using .str.strip().str.lower().str.title() to make everything consistent and neat (e.g., “usa ” becomes “Usa”).

#5.Formatted Dates Consistently
The date_added column had inconsistent or unclear formats like "September 9, 2019". I converted it into a uniform dd-mm-yyyy format so it’s easy to sort, filter, or analyze.

#6.Renamed Column Headers
To make the columns easier to use in code, I renamed them to all lowercase and replaced spaces with underscores (e.g., Date Added → date_added).
