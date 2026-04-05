ex-11
Nikunj Deep Upadhyay
Entc b1
Title : Dataset Creation

Theory This experiment focuses on performing data creation, loading, exploration, and preprocessing using Pandas in Python, which is widely used for data analysis and data science tasks. 🔹 1. DataFrame and Dataset Creation A DataFrame is a two-dimensional, tabular data structure consisting of rows and columns. In this experiment, a dataset (students.csv) is created using a Python dictionary. Each key represents a column (Roll_No, Gender, Department, CGPA), and values represent the data entries. The dataset is then exported to a CSV file using to_csv(), which allows data storage and reuse.

 2. Data Loading External datasets (like Cars93) are loaded using pd.read_csv(). This dataset contains 93 rows and 10 columns, including both numerical and categorical data such as: Manufacturer, Model, Type (categorical) Price, MPG.city, Horsepower (numerical) Loading data is the first step in real-world data analysis.

 3. Data Exploration (EDA – Exploratory Data Analysis) EDA is used to understand the structure and characteristics of the dataset. Important Functions: df.head() and df.tail() → View first and last records df.shape → Returns number of rows and columns df.size → Total number of elements df.columns → Lists column names df.sample() → Random sampling of data These functions help in quickly inspecting the dataset.

 4. Data Information and Types df.info() provides: Number of non-null values Data types (int, float, object) Numerical columns: Price, MPG.city, Horsepower Categorical columns: Manufacturer, Model, Type Understanding data types is important for analysis and model building.

 5. Statistical Summary df.describe() generates summary statistics such as: Mean, median, standard deviation Minimum and maximum values Example insights: Average car price ≈ 19.51 Average horsepower ≈ 143.83 MPG varies between 15 and 46 This helps in understanding data distribution.

 6. Data Cleaning Data cleaning ensures data quality before analysis. Missing Values: Checked using df.isnull().sum() Missing values found in: AirBags (34 values) Rear.seat.room (2 values) Luggage.room (11 values) Duplicate Records: Checked using df.duplicated().sum() No duplicate records found Unique Values: df.nunique() shows diversity of data Example: 32 manufacturers, 6 types of cars

 7. Importance of Data Preprocessing Handling missing values (fill/drop) Converting data types if needed Removing inconsistencies This step improves data quality and ensures better results in analysis or machine learning.

Conclusion Pandas provides efficient tools for data handling, exploration, and preprocessing. The student dataset demonstrates data creation and storage, while the Cars dataset shows real-world data analysis. The dataset is mostly clean (no duplicates) but contains missing values, which must be handled. Statistical analysis helps in extracting meaningful insights like average price
