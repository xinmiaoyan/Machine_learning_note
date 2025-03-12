# Machine_learning_note
## 1. resources
### 1) [Python](https://www.python.org/) 
1.1-python.md
### 2) 🐼 [pandas](https://pandas.pydata.org/)
pandas provides high-level data structures and functions designed to make working with structured or tabular data fast, easy, and expressive. Since its emergence in 2010, it has helped enable Python to be a powerful and productive data analysis environment. The primary objects in pandas that will be used in this book are the DataFrame, a tabular, column-oriented data structure with both row and column labels, and the Series, a one-dimensional labeled array object.
pandas blends the high-performance, array-computing ideas of NumPy with the flex‐ ible data manipulation capabilities of spreadsheets and relational databases (such as SQL). It provides sophisticated indexing functionality to make it easy to reshape, slice and dice, perform aggregations, and select subsets of data.
* Data structures with labeled axes supporting automatic or explicit data alignment, this prevents common errors resulting from misaligned data and working with differently indexed data coming from different sources
* Integrated time series functionality
* The same data structures handle both time series data and non–time series data
* Arithmetic operations and reductions that preserve metadata
* Flexible handling of missing data
* Merge and other relational operations found in popular databases (SQL-based, for example)
### 3) [numpy](https://numpy.org/)
NumPy, short for Numerical Python, has long been a cornerstone of numerical computing in Python. It provides the data structures, algorithms, and tools needed for most scientific applications involving numerical data in Python. NumPy contains, among other things:

* A fast and efficient multidimensional array object ndarray
* Functions for performing element-wise computations with arrays or mathematical operations between arrays
* Tools for reading and writing array-based datasets to disk
* Linear algebra operations, Fourier transform, and random number generation
* A mature C API to enable Python extensions and native C or C++ code to access NumPy's data structures and computational facilities

Beyond the fast array-processing capabilities that NumPy adds to Python, one of its primary uses in data analysis is as a container for data to be passed between algorithms and libraries. For numerical data, NumPy arrays are more efficient for storing and manipulating data than the other built-in Python data types. Also, libraries written in a lower-level language, such as C or Fortran, can operate on the data stored in a NumPy array without copying data into a separate memory representation. Thus, many numerical computing tools for Python either assume NumPy arrays as a primary data structure or else target seamless interoperability with NumPy.

### 4) [matplotlib](https://matplotlib.org/)
matplotlib is the most popular Python library for producing plots and other two- dimensional data visualizations. It was originally created by John D. Hunter and is now maintained by a large team of developers. It is designed for creating plots suit‐ able for publication. While there are other visualization libraries available to Python programmers, matplotlib is the most widely used and as such has generally good integration with the rest of the ecosystem. I think it is a safe choice as a default visualization tool.
### 5) [SciPy](https://scipy.org/)
SciPy is a collection of packages addressing a number of different standard problem domains in scientific computing. Here is a sampling of the packages included:
#### scipy.integrate
Numerical integration routines and differential equation solvers
#### scipy.linalg
Linear algebra routines and matrix decompositions extending beyond those pro‐ vided in numpy.linalg
#### scipy.optimize
Function optimizers (minimizers) and root finding algorithms
#### scipy.signal
Signal processing tools
#### scipy.sparse
Sparse matrices and sparse linear system solvers
#### scipy.special
Wrapper around SPECFUN, a Fortran library implementing many common mathematical functions, such as the gamma function
#### scipy.stats
Standard continuous and discrete probability distributions (density functions, samplers, continuous distribution functions), various statistical tests, and more descriptive statistics
Together NumPy and SciPy form a reasonably complete and mature computational foundation for many traditional scientific computing applications.
### 6) [scikit-learn](https://scikit-learn.org/stable/)
Since the project’s inception in 2010, scikit-learn has become the premier general- purpose machine learning toolkit for Python programmers. In just seven years, it has had over 1,500 contributors from around the world. It includes submodules for such models as:
* Classification: SVM, nearest neighbors, random forest, logistic regression, etc.
* Regression: Lasso, ridge regression, etc.
* Clustering: k-means, spectral clustering, etc.
* Dimensionality reduction: PCA, feature selection, matrix factorization, etc.
* Model selection: Grid search, cross-validation, metrics
* Preprocessing: Feature extraction, normalization
Along with pandas, statsmodels, and IPython, scikit-learn has been critical for ena‐ bling Python to be a productive data science programming language.
### 7) [statsmodels](https://www.statsmodels.org/stable/index.html)
statsmodels is a statistical analysis package that was seeded by work from Stanford University statistics professor Jonathan Taylor, who implemented a number of regression analysis models popular in the R programming language. Skipper Seabold and Josef Perktold formally created the new statsmodels project in 2010 and since then have grown the project to a critical mass of engaged users and contributors. Nathaniel Smith developed the Patsy project, which provides a formula or model specification framework for statsmodels inspired by R’s formula system.
Compared with scikit-learn, statsmodels contains algorithms for classical (primarily frequentist) statistics and econometrics. This includes such submodules as:
* Regression models: Linear regression, generalized linear models, robust linear models, linear mixed effects models, etc.
* Analysis of variance (ANOVA)
* Time series analysis: AR, ARMA, ARIMA, VAR, and other models
* Nonparametric methods: Kernel density estimation, kernel regression
* Visualization of statistical model results
statsmodels is more focused on statistical inference, providing uncertainty estimates and p-values for parameters. scikit-learn, by contrast, is more prediction-focused.
### 8) [seaborn](https://seaborn.pydata.org/)
