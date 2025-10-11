# NumPy Assignment: Banking Industry Analysis — Questions Only

# Dataset Overview
# Columns:
# 1. Customer_ID – Unique identifier for each customer
# 2. Account_Balance – Customer's account balance ($)
# 3. Credit_Score – Credit score (300–900)
# 4. Transaction_Count – Transactions in the last month
# 5. Years_Active – Years with the bank

# -----------------------------------------------------------
# Question 1: Array Creation and Manipulation
# -----------------------------------------------------------
# Q1.1 Create a 4x4 identity matrix using np.eye()
# Q1.2 Create an array of 8 zeros using np.zeros()
# Q1.3 Create an array of 6 ones using np.ones()
# Q1.4 Create an array with values from 0 to 15 using np.arange()
# Q1.5 Create an array with 8 evenly spaced values from 0 to 100 using np.linspace()

# -----------------------------------------------------------
# Question 2: Array Attributes and Information
# -----------------------------------------------------------
# Q2.1 Find the shape of banking_data
# Q2.2 Find the data type of banking_data
# Q2.3 Find the total number of elements (size)
# Q2.4 Find the number of dimensions
# Q2.5 Find the memory size (in bytes)

# -----------------------------------------------------------
# Question 3: Indexing and Slicing
# -----------------------------------------------------------
# Q3.1 Extract the first row of banking_data
# Q3.2 Extract the last row of banking_data
# Q3.3 Extract the Account_Balance column
# Q3.4 Extract the first 4 rows and first 3 columns
# Q3.5 Extract rows 3 to 7 (inclusive)

# -----------------------------------------------------------
# Question 4: Mathematical Operations
# -----------------------------------------------------------
# Q4.1 Calculate sum of all account balances
# Q4.2 Calculate mean account balance
# Q4.3 Calculate standard deviation of balances
# Q4.4 Calculate variance of balances
# Q4.5 Calculate median account balance

# -----------------------------------------------------------
# Question 5: Statistical Functions
# -----------------------------------------------------------
# Q5.1 Find min and max account balances
# Q5.2 Find min and max credit scores
# Q5.3 Percentiles (25th, 50th, 75th) of balances
# Q5.4 Correlation between balance and credit score
# Q5.5 Covariance between balance and credit score

# -----------------------------------------------------------
# Question 6: Array Reshaping and Manipulation
# -----------------------------------------------------------
# Q6.1 Reshape banking_data to 5x10
# Q6.2 Flatten banking_data to 1D
# Q6.3 Transpose banking_data
# Q6.4 Split into 2 vertical parts
# Q6.5 Split into 2 horizontal parts

# -----------------------------------------------------------
# Question 7: Logical Operations and Filtering
# -----------------------------------------------------------
# Q7.1 Customers with balance > 100000
# Q7.2 Customers with credit score > 800
# Q7.3 Transactions > 50 AND credit score < 750
# Q7.4 Count customers with balance between 10000 and 100000
# Q7.5 Index of customer with highest credit score

# -----------------------------------------------------------
# Question 8: Sorting and Searching
# -----------------------------------------------------------
# Q8.1 Sort by account balance (ascending)
# Q8.2 Sort by credit score (descending)
# Q8.3 Indices that would sort by years active
# Q8.4 Find second highest balance
# Q8.5 Find customer with lowest transaction count

# -----------------------------------------------------------
# Question 9: Mathematical Functions
# -----------------------------------------------------------
# Q9.1 Absolute values of all elements
# Q9.2 Square root of account balances
# Q9.3 Square of credit scores
# Q9.4 Exponential of transaction counts
# Q9.5 Natural log of account balances

# -----------------------------------------------------------
# Question 10: Advanced Operations
# -----------------------------------------------------------
# Q10.1 Cumulative sum of balances
# Q10.2 Cumulative product of transaction counts
# Q10.3 Difference between consecutive balances
# Q10.4 Gradient of account balances
# Q10.5 Histogram of balances with 5 bins

# -----------------------------------------------------------
# Question 11: Random Numbers and Simulation
# -----------------------------------------------------------
# Q11.1 Generate 6 random integers (1–1000)
# Q11.2 Generate 6 random floats (0–1)
# Q11.3 Generate 6 random normal numbers (mean=700, std=100)
# Q11.4 Shuffle banking_data rows
# Q11.5 Set seed (123) and generate 4 random numbers

# -----------------------------------------------------------
# Question 12: Linear Algebra Operations
# -----------------------------------------------------------
# Q12.1 Dot product of account balance and credit score
# Q12.2 Cross product of first two rows
# Q12.3 Norm of account balance column
# Q12.4 Determinant of 3x3 matrix
# Q12.5 Inverse of 3x3 matrix

# -----------------------------------------------------------
# Question 13: String Operations
# -----------------------------------------------------------
# Q13.1 Convert Customer_IDs to strings
# Q13.2 Check if any ID contains '100'
# Q13.3 Convert IDs to uppercase
# Q13.4 Count length of each ID string
# Q13.5 Replace '100' with 'CUST' in IDs

# -----------------------------------------------------------
# Question 14: Date and Time Operations
# -----------------------------------------------------------
# Q14.1 Convert years active to months
# Q14.2 Average years active
# Q14.3 Customers active > 5 years
# Q14.4 Total years active (sum)
# Q14.5 Customer with shortest tenure

# -----------------------------------------------------------
# Question 15: Advanced Array Operations
# -----------------------------------------------------------
# Q15.1 Apply 5% interest on balances
# Q15.2 Categorize by balance (np.where)
# Q15.3 Categorize by credit score (np.select)
# Q15.4 Apply different rates by balance (np.piecewise)
# Q15.5 Sum each row using np.apply_along_axis

# -----------------------------------------------------------
# Question 16: Array Concatenation and Stacking
# -----------------------------------------------------------
# Q16.1 Concatenate horizontally (np.hstack)
# Q16.2 Concatenate vertically (np.vstack)
# Q16.3 Concatenate along axis (np.concatenate)
# Q16.4 Stack depth-wise (np.dstack)
# Q16.5 Column stack (np.column_stack)

# -----------------------------------------------------------
# Question 17: Array Splitting Operations
# -----------------------------------------------------------
# Q17.1 Split into 3 equal parts (np.split)
# Q17.2 Split at specific indices
# Q17.3 Horizontal split (np.hsplit)
# Q17.4 Vertical split (np.vsplit)
# Q17.5 Split into chunks (np.array_split)

# -----------------------------------------------------------
# Question 18: Array Repetition and Tiling
# -----------------------------------------------------------
# Q18.1 Repeat each element 3 times
# Q18.2 Repeat entire array twice
# Q18.3 Repeat 2D array (np.tile)
# Q18.4 Create pattern with np.tile
# Q18.5 Repeat elements with different counts

# -----------------------------------------------------------
# Question 19: Array Comparison and Logical Operations
# -----------------------------------------------------------
# Q19.1 Compare two arrays (np.array_equal)
# Q19.2 Check closeness (np.allclose)
# Q19.3 Logical AND between arrays
# Q19.4 Logical OR between arrays
# Q19.5 Logical NOT on an array

# -----------------------------------------------------------
# Question 20: Array Set Operations
# -----------------------------------------------------------
# Q20.1 Unique elements (np.unique)
# Q20.2 Intersection (np.intersect1d)
# Q20.3 Union (np.union1d)
# Q20.4 Difference (np.setdiff1d)
# Q20.5 Symmetric difference (np.setxor1d)

# -----------------------------------------------------------
# Learning Objectives:
# - Master NumPy operations and analysis
# - Perform statistical, logical, and linear algebra operations
# - Manipulate real-world financial datasets efficiently
# - Build confidence with vectorized computations

# -----------------------------------------------------------
# Expected Outcomes:
# - Analyze banking data with NumPy
# - Apply statistical and mathematical operations
# - Perform transformations and filtering
# - Derive insights into customer trends
