# NumPy Practice — Complete NumPy Roadmap for Data Science & Machine Learning

A structured, hands-on NumPy learning repository covering 16 essential topics, from array fundamentals to linear algebra, numerical computing, and practical Machine Learning applications.

This repository is designed to build a strong numerical computing foundation for **Data Science, Machine Learning, Deep Learning, and AI Engineering** through practical examples, code implementations, and progressive learning.

---

## 📌 Table of Contents

* [About the Repository](#-about-the-repository)
* [Learning Objectives](#-learning-objectives)
* [Tech Stack](#-tech-stack)
* [Repository Structure](#-repository-structure)
* [Installation & Setup](#-installation--setup)
* [Complete NumPy Roadmap](#-complete-numpy-roadmap)
* [Learning Progress](#-learning-progress)
* [Machine Learning Applications](#-machine-learning-applications)
* [Learning Path](#-learning-path)
* [How to Use This Repository](#-how-to-use-this-repository)
* [Resources](#-resources)
* [Author](#-author)

---

## 📖 About the Repository

NumPy (Numerical Python) is a fundamental Python library for numerical computing. It provides powerful multidimensional arrays, mathematical operations, broadcasting, vectorization, statistical functions, and linear algebra tools.

This repository contains my NumPy practice, organized into a structured roadmap of 16 important topics.

The primary goal is to develop practical NumPy skills for working with numerical datasets, implementing mathematical operations, and understanding the underlying concepts used in Machine Learning algorithms.

---

## 🎯 Learning Objectives

By completing this repository, I aim to:

* Understand NumPy arrays and multidimensional data structures.
* Perform array indexing, slicing, filtering, and reshaping.
* Work efficiently with NumPy data types and memory.
* Apply broadcasting and vectorization for numerical computations.
* Perform mathematical, statistical, and aggregation operations.
* Understand random sampling and probability distributions.
* Implement linear algebra operations using `numpy.linalg`.
* Process numerical datasets for Data Science and Machine Learning.
* Build a strong foundation for Pandas, SciPy, and Scikit-learn.

---

## 🛠️ Tech Stack

| Technology                   | Purpose                                  |
| ---------------------------- | ---------------------------------------- |
| Python                       | Core programming language                |
| NumPy                        | Numerical computing and array operations |
| Jupyter Notebook             | Interactive coding and practice          |
| Git & GitHub                 | Version control and project management   |
| Virtual Environment (`venv`) | Dependency isolation                     |

---

## 📂 Repository Structure

```text
numpy-practice/
│
├── notebooks/
│   ├── 01_numpy_fundamentals.ipynb
│   ├── 02_array_creation.ipynb
│   ├── 03_data_types_conversion.ipynb
│   ├── 04_indexing_selection.ipynb
│   ├── 05_array_slicing.ipynb
│   ├── 06_boolean_fancy_indexing.ipynb
│   ├── 07_reshaping_dimensions.ipynb
│   ├── 08_joining_splitting.ipynb
│   ├── 09_copy_view_memory.ipynb
│   ├── 10_broadcasting_vectorization.ipynb
│   ├── 11_math_ufunc.ipynb
│   ├── 12_statistics_aggregation.ipynb
│   ├── 13_sorting_searching.ipynb
│   ├── 14_random_probability.ipynb
│   ├── 15_linear_algebra.ipynb
│   └── 16_numpy_for_data_science_ml.ipynb
│
├── datasets/
│   └── .gitkeep
│
├── exercises/
│   └── .gitkeep
│
├── projects/
│   └── .gitkeep
│
├── images/
│   └── .gitkeep
│
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/numpy-practice.git

cd numpy-practice
```

### 2. Create a Virtual Environment

```bash
python3 -m venv .venv
```

### 3. Activate the Virtual Environment

**Ubuntu / Linux / macOS**

```bash
source .venv/bin/activate
```

**Windows (PowerShell)**

```powershell
.venv\Scripts\Activate.ps1
```

### 4. Upgrade pip

```bash
python -m pip install --upgrade pip
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Register the Jupyter Kernel

```bash
python -m ipykernel install --user --name=numpy-practice --display-name "Python (NumPy Practice)"
```

### 7. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the `notebooks/` directory and start practicing.

---

## 📚 Complete NumPy Roadmap

The following 16 topics cover the core NumPy skills I am practicing for Data Science and Machine Learning.

### 🟢 01. NumPy Fundamentals

**Topics Covered:**

* What is NumPy?
* Why use NumPy?
* Features and applications of NumPy
* Importing NumPy using `import numpy as np`
* NumPy `ndarray`
* 1D, 2D, 3D, and N-dimensional arrays
* Array attributes: `ndim`, `shape`, `size`, `dtype`

**Important Attributes & Functions:**

```python
np.array()
arr.ndim
arr.shape
arr.size
arr.dtype
```

**Machine Learning Connection:** Understanding feature matrices (`X`) and target vectors (`y`).

---

### 🟢 02. Array Creation

**Topics Covered:**

* Creating arrays from Python lists and tuples
* Arrays with specific values
* Zero, one, and constant-filled arrays
* Empty arrays
* Range-based arrays
* Evenly spaced values
* Identity matrices

**Important Functions:**

```python
np.array()
np.zeros()
np.ones()
np.full()
np.empty()
np.arange()
np.linspace()
np.eye()
```

**Example:**

```python
import numpy as np

a = np.array([10, 20, 30])
b = np.zeros(5)
c = np.ones((2, 3))
d = np.arange(1, 10)
```

**Machine Learning Connection:** Creating feature arrays, initializing weights, and generating numerical data.

---

### 🟢 03. Data Types & Type Conversion

**Topics Covered:**

* NumPy `dtype`
* Integer, float, Boolean, and complex data types
* Data type conversion
* Using `astype()`
* Selecting appropriate data types
* Data type and memory consumption

**Important Attributes & Methods:**

```python
arr.dtype
arr.astype(float)
arr.astype(int)
```

**Machine Learning Connection:** Numerical data preprocessing and memory-efficient data representation.

---

### 🟡 04. Array Indexing & Selection

**Topics Covered:**

* Positive and negative indexing
* 1D, 2D, and 3D array indexing
* Row and column selection
* Multidimensional indexing
* Selecting specific elements

**Examples:**

```python
arr[0]
arr[-1]
arr[0, 1]
arr[:, 0]
arr[1, :]
```

**Machine Learning Connection:** Selecting individual samples, rows, and features from a dataset.

---

### 🟡 05. Array Slicing

**Topics Covered:**

* Start, stop, and step
* 1D and 2D slicing
* Row and column slicing
* Reverse slicing
* Slice assignment
* Understanding slice views

**Syntax:**

```python
array[start:stop:step]
```

**Examples:**

```python
arr[1:5]
arr[:3]
arr[::2]
arr[::-1]

arr[0:2, 1:3]
```

**Machine Learning Connection:** Extracting dataset subsets and selecting feature ranges.

---

### 🟡 06. Boolean & Fancy Indexing

**Topics Covered:**

* Boolean conditions and masks
* Filtering arrays
* Multiple conditions
* AND (`&`), OR (`|`), and NOT (`~`)
* Integer-array indexing
* Selecting specific rows and elements

**Examples:**

```python
arr[arr > 50]

arr[(arr > 20) & (arr < 80)]

arr[[0, 2, 4]]
```

**Machine Learning Connection:** Dataset filtering, outlier selection, and condition-based data processing.

---

### 🟠 07. Reshaping & Dimension Manipulation

**Topics Covered:**

* `reshape()`
* `reshape(-1)`
* Shape compatibility
* 1D → 2D → 3D transformations
* `flatten()` and `ravel()`
* `expand_dims()` and `squeeze()`

**Examples:**

```python
arr.reshape(2, 3)
arr.reshape(-1)

arr.flatten()
arr.ravel()

np.expand_dims(arr, axis=0)
np.squeeze(arr)
```

**Machine Learning Connection:** Preparing feature matrices and reshaping input data for ML and DL models.

```python
# Convert a 1D array into a column vector
X = np.array([10, 20, 30])

X = X.reshape(-1, 1)

print(X.shape)  # (3, 1)
```

---

### 🟠 08. Array Joining & Splitting

**Topics Covered:**

* Joining arrays
* `concatenate()`
* `stack()`
* `hstack()` and `vstack()`
* Joining arrays along different axes
* `split()` and `array_split()`
* `hsplit()` and `vsplit()`

**Examples:**

```python
np.concatenate([a, b])

np.vstack([a, b])
np.hstack([a, b])

np.split(arr, 2)
np.array_split(arr, 3)
```

**Machine Learning Connection:** Combining features, assembling arrays, and splitting numerical data.

---

### 🔵 09. Copy, View & Memory

**Topics Covered:**

* Understanding views and copies
* `view()` and `copy()`
* Shared memory
* The `base` attribute
* `shares_memory()`
* Array memory consumption using `nbytes`

**Examples:**

```python
b = a.view()
c = a.copy()

np.shares_memory(a, b)

a.nbytes
```

**Key Difference:**

| View                            | Copy                               |
| ------------------------------- | ---------------------------------- |
| Shares underlying data          | Creates independent data           |
| Changes may affect the original | Changes do not affect the original |
| Often avoids data duplication   | Requires additional memory         |

**Machine Learning Connection:** Memory management and efficient manipulation of large numerical datasets.

---

### 🔥 10. Broadcasting & Vectorization

**Topics Covered:**

* Broadcasting fundamentals
* Broadcasting rules
* Scalar and array broadcasting
* 1D and 2D broadcasting
* Broadcasting errors
* Vectorized operations
* Array arithmetic without explicit Python loops

**Examples:**

```python
arr + 10
arr * 2
```

Instead of:

```python
for i in range(len(arr)):
    arr[i] *= 2
```

**Key Concept:**

Broadcasting allows compatible array shapes to work together, while vectorization applies operations across arrays without writing explicit element-by-element Python loops.

**Machine Learning Connection:** Efficient numerical calculations, feature transformations, and mathematical operations.

---

### 🔥 11. Mathematical Operations & Universal Functions (ufunc)

**Topics Covered:**

* Addition, subtraction, multiplication, and division
* Power and absolute value
* Square and square root
* Unary and binary universal functions
* Exponential and logarithmic functions
* Minimum and maximum
* Floor and ceiling

**Important Functions:**

```python
np.add(a, b)
np.subtract(a, b)
np.multiply(a, b)
np.divide(a, b)

np.sqrt(a)
np.square(a)
np.exp(a)
np.log(a)

np.maximum(a, b)
np.minimum(a, b)

np.floor(a)
np.ceil(a)
```

**Machine Learning Connection:** Mathematical transformations, loss calculations, and numerical operations used in ML algorithms.

---

### 🔥 12. Statistics & Aggregation

**Topics Covered:**

* Mean, median, standard deviation, and variance
* Minimum and maximum
* Percentile and quantile
* `argmin()` and `argmax()`
* Sum and product
* Cumulative sum and product
* Aggregation along different axes

**Important Functions:**

```python
np.mean(arr)
np.median(arr)
np.std(arr)
np.var(arr)

np.min(arr)
np.max(arr)

np.percentile(arr, 50)
np.quantile(arr, 0.5)

np.sum(arr)
np.prod(arr)

np.cumsum(arr)
np.cumprod(arr)

np.argmin(arr)
np.argmax(arr)
```

**Understanding Axis:**

```python
np.mean(arr, axis=0)  # Aggregate along rows, per column
np.mean(arr, axis=1)  # Aggregate along columns, per row
```

**Machine Learning Connection:** Descriptive statistics, feature analysis, and numerical summaries.

---

### 🔵 13. Sorting, Searching & Filtering

**Topics Covered:**

* Array sorting
* Sorting along different axes
* Descending sorting
* `argsort()`
* Searching with conditions
* `where()` and `nonzero()`
* `searchsorted()`
* Top-N selection with `argpartition()`

**Important Functions:**

```python
np.sort(arr)
np.argsort(arr)

np.where(arr > 50)
np.nonzero(arr)

np.searchsorted(arr, 30)
np.argpartition(arr, -3)
```

**Machine Learning Connection:** Ranking predictions, selecting top-N values, and analyzing numerical data.

---

### 🟣 14. Random & Probability

**Topics Covered:**

* NumPy random module
* Random seeds and reproducibility
* Modern random generator using `default_rng()`
* Random floats and integers
* Random sampling using `choice()`
* Shuffle and permutation
* Uniform, normal, binomial, Poisson, and exponential distributions

**Examples:**

```python
rng = np.random.default_rng(42)

rng.random(5)
rng.integers(1, 100, size=5)

rng.choice([10, 20, 30], size=5)

rng.normal(0, 1, size=100)
rng.uniform(0, 1, size=100)
```

**Machine Learning Connection:** Random sampling, reproducible experiments, synthetic data generation, and simulation.

---

### 🔵 15. Linear Algebra for Machine Learning

**Topics Covered:**

* Vectors and matrices
* Matrix shapes and dimensions
* Matrix addition and multiplication
* Matrix transpose
* Dot, inner, and outer products
* Trace, rank, determinant, inverse, and norm
* Solving linear equations
* Eigenvalues and eigenvectors
* Singular Value Decomposition (SVD)

**Important Functions:**

```python
np.dot(a, b)
np.matmul(a, b)

np.trace(A)
np.linalg.det(A)
np.linalg.inv(A)
np.linalg.matrix_rank(A)
np.linalg.norm(A)

np.linalg.solve(A, b)

np.linalg.eig(A)
np.linalg.svd(A)
```

**Machine Learning Connection:** Linear Regression, matrix-based computations, optimization, and Principal Component Analysis (PCA).

---

### 🔥 16. NumPy for Data Science & Machine Learning

**Topics Covered:**

**Data Science & Preprocessing**

* Numerical data processing
* Missing-value handling with `np.nan`
* Statistical analysis
* Outlier detection
* Normalization and standardization
* Min-Max scaling
* Feature transformation
* Correlation and covariance

**ML Data Representation**

* Feature matrix (`X`)
* Target vector (`y`)
* Dataset shape and dimensions
* Numerical feature selection

**ML Mathematics**

* Dot product and matrix multiplication
* Distance calculations
* Loss functions
* Mean Squared Error (MSE)
* Gradient descent
* Weight updates

**NumPy + Pandas Workflow**

```text
NumPy Arrays
     ↓
Pandas Series & DataFrames
     ↓
Data Preprocessing
     ↓
Exploratory Data Analysis
     ↓
Scikit-learn
     ↓
Machine Learning Models
```

**Example:**

```python
import numpy as np

X = np.array([
    [20, 50000],
    [25, 60000],
    [30, 75000]
])

y = np.array([0, 1, 1])

print("Feature Matrix:", X.shape)
print("Target Vector:", y.shape)
```

**Machine Learning Connection:** Applying NumPy concepts to real-world numerical datasets and understanding the mathematical foundations of ML algorithms.

---

## 📊 Learning Progress

Track my progress through the 16 core NumPy topics.

* [ ] 01. NumPy Fundamentals
* [ ] 02. Array Creation
* [ ] 03. Data Types & Type Conversion
* [ ] 04. Array Indexing & Selection
* [ ] 05. Array Slicing
* [ ] 06. Boolean & Fancy Indexing
* [ ] 07. Reshaping & Dimension Manipulation
* [ ] 08. Array Joining & Splitting
* [ ] 09. Copy, View & Memory
* [ ] 10. Broadcasting & Vectorization
* [ ] 11. Mathematical Operations & ufunc
* [ ] 12. Statistics & Aggregation
* [ ] 13. Sorting, Searching & Filtering
* [ ] 14. Random & Probability
* [ ] 15. Linear Algebra for Machine Learning
* [ ] 16. NumPy for Data Science & Machine Learning

---

## 🧠 Machine Learning Applications

This repository builds the numerical computing foundation required for:

| Application               | NumPy Concepts                                 |
| ------------------------- | ---------------------------------------------- |
| Feature Engineering       | Indexing, slicing, broadcasting                |
| Data Preprocessing        | Filtering, statistics, transformations         |
| Linear Regression         | Matrix multiplication, dot product             |
| Gradient Descent          | Vectorization, arithmetic, aggregation         |
| Model Evaluation          | MSE, statistical operations                    |
| PCA                       | Linear algebra, eigenvalues, SVD               |
| Neural Networks           | Matrix operations, broadcasting, vectorization |
| Synthetic Data Generation | Random sampling, probability distributions     |

---

## 🗺️ Learning Path

My planned learning sequence:

```text
NumPy Fundamentals
        ↓
Array Creation & Data Types
        ↓
Indexing, Slicing & Filtering
        ↓
Reshaping & Dimension Manipulation
        ↓
Joining, Splitting & Memory
        ↓
Broadcasting & Vectorization
        ↓
Mathematical Operations & Statistics
        ↓
Sorting, Searching & Random
        ↓
Linear Algebra
        ↓
NumPy for Data Science & Machine Learning
        ↓
Pandas → Matplotlib → Seaborn → SciPy
        ↓
Scikit-learn → Machine Learning Projects
```

---

## 💻 How to Use This Repository

1. Follow the notebooks in numerical order.
2. Read the concept explanations and code examples.
3. Execute the code cells and experiment with different inputs.
4. Complete the exercises after each topic.
5. Practice with numerical datasets.
6. Build small projects using the concepts learned.
7. Update the learning progress checklist as topics are completed.

---

## 📚 Resources

* [NumPy Official Documentation](https://numpy.org/doc/)
* [NumPy User Guide](https://numpy.org/doc/stable/user/)
* [NumPy API Reference](https://numpy.org/doc/stable/reference/)
* [NumPy Quickstart Tutorial](https://numpy.org/doc/stable/user/quickstart.html)
* [NumPy Absolute Beginners Guide](https://numpy.org/doc/stable/user/absolute_beginners.html)

---

## 👨‍💻 Author

**Md. Shagor Ali**

Aspiring AI/ML Engineer | Machine Learning | Deep Learning | Computer Vision | NLP | LLMs | Generative AI | AI Agents

BSc in Computer Science & Engineering

Green University of Bangladesh

### Connect with Me

* GitHub: https://github.com/shagor186
* LinkedIn: www.linkedin.com/in/shagor186


---

## ⭐ Support

If you find this repository useful for learning NumPy, Data Science, or Machine Learning, consider giving it a ⭐ on GitHub.

This repository is part of my continuous journey toward becoming an AI/ML Engineer through consistent practice, hands-on projects, and learning.