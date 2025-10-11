# =====================================================
# NumPy Course: Detailed Syllabus with Explanations and Examples
# =====================================================

# -----------------------------------------------------
# Module 1: Introduction to NumPy
# -----------------------------------------------------

# 1.1 Context: Numerical Computing in Python
# NumPy enables fast, efficient computation on large numerical datasets using arrays and matrices.

# 1.2 Limitations of Standard Python Lists
# - Slow for large data (loops in Python)
# - High memory usage
# - Lack of built-in mathematical operations

# 1.3 NumPy's Core Contribution: ndarray
# The ndarray is a fast, memory-efficient container for homogeneous data.

# 1.4 Performance Advantages: Vectorization
# Vectorized operations avoid Python loops and execute C-compiled code for speed.

# Example:
import numpy as np
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = a + b
print(c)  # Output: [5 7 9]

# 1.5 Key Application Areas
# Data Science, Machine Learning, AI, Scientific Computing, Finance

# 1.6 Installation
# pip install numpy
# conda install numpy

# 1.7 Import Convention
import numpy as np
my_array = np.array([1, 2, 3])
print(my_array)  # [1 2 3]


# -----------------------------------------------------
# Module 2: NumPy Arrays (ndarray)
# -----------------------------------------------------

# 2.1 ndarray Object
# Homogeneous, fixed-size N-dimensional array

# 2.2 Creating Arrays
vector = np.array([1, 2, 3])
matrix = np.array([[1, 2], [3, 4]])
tensor = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])
print(vector, matrix, tensor)

# 2.3 Arrays vs. Lists
import time
size = 1_000_000
lst1 = list(range(size))
lst2 = list(range(size))
arr1 = np.arange(size)
arr2 = np.arange(size)

# List addition
start = time.time()
list_result = [x + y for x, y in zip(lst1, lst2)]
print("List time:", time.time() - start)

# NumPy addition
start = time.time()
arr_result = arr1 + arr2
print("NumPy time:", time.time() - start)

# 2.4 Data Types (dtype)
float_arr = np.array([1, 2, 3], dtype=np.float32)
complex_arr = np.array([1+2j, 3+4j])
print(float_arr.dtype, complex_arr.dtype)

# 2.5 Array Attributes
mat = np.array([[1, 2], [3, 4], [5, 6]], dtype=np.float32)
print(mat.ndim, mat.shape, mat.size, mat.dtype, mat.itemsize, mat.nbytes)

# 2.6 Data Type Conversion
int_arr = np.array([1, 2, 3])
float_arr = int_arr.astype(np.float64)
print(float_arr)
bool_arr = np.array([0, 1, 2]).astype(np.bool_)
print(bool_arr)


# -----------------------------------------------------
# Module 3: Array Creation Techniques
# -----------------------------------------------------

# 3.2 Arrays with specific values
zeros = np.zeros((2, 3))
ones = np.ones((2, 3))
empty = np.empty((2, 2))
full = np.full((2, 2), 7)
eye = np.eye(3)
print(zeros, ones, full, eye)

# 3.3 Numerical Ranges
arange_ex = np.arange(0, 10, 2)
lin_ex = np.linspace(0, 1, 5)
log_ex = np.logspace(0, 3, 4)
geom_ex = np.geomspace(1, 1000, 4)
print(arange_ex, lin_ex, log_ex, geom_ex)

# 3.4 Random Arrays
rand = np.random.rand(2, 3)
randint = np.random.randint(1, 10, (3, 3))
choice = np.random.choice(['A', 'B', 'C'], 5, p=[0.5, 0.3, 0.2])
print(rand, randint, choice)

rng = np.random.default_rng(42)
print(rng.integers(1, 10, size=5))
arr = np.arange(5)
rng.shuffle(arr)
print(arr)


# -----------------------------------------------------
# Module 4: Indexing and Slicing
# -----------------------------------------------------

# 4.1 Basic Indexing
vec = np.arange(10)
print(vec[3])       # 3
mat = np.array([[1, 2], [3, 4]])
print(mat[1, 0])    # 3

# 4.2 Basic Slicing
arr = np.arange(10)
print(arr[2:6])     # [2 3 4 5]
mat = np.arange(12).reshape(3, 4)
print(mat[:2, 1:3]) # submatrix

# View vs Copy
a = np.arange(5)
b = a[1:4]
b[0] = 99
print(a)  # modifies original
c = a[1:4].copy()
c[0] = 0
print(a)  # original unchanged

# 4.3 Advanced Indexing
# Boolean indexing
arr = np.arange(10)
mask = arr > 5
print(arr[mask])  # [6 7 8 9]

# Fancy indexing
mat = np.arange(16).reshape(4, 4)
print(mat[[0, 2], [1, 3]])  # select elements (0,1), (2,3)

# -----------------------------------------------------
# End of Modules 1–4
# (Modules 5–11 continue in same style)
# -----------------------------------------------------
