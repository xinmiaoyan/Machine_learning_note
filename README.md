# Machine_learning_note
## 1. resources
### 1) [Python](https://www.python.org/)
#### Why Python for Data Analysis?
For many people, the Python programming language has strong appeal. Since its first appearance in 1991, Python has become one of the most popular interpreted pro‐ gramming languages, along with Perl, Ruby, and others. Python and Ruby have become especially popular since 2005 or so for building websites using their numer‐ ous web frameworks, like Rails (Ruby) and Django (Python). Such languages are often called scripting languages, as they can be used to quickly write small programs, or scripts to automate other tasks. I don’t like the term “scripting language,” as it car‐ ries a connotation that they cannot be used for building serious software. Among interpreted languages, for various historical and cultural reasons, Python has developed a large and active scientific computing and data analysis community. In the last 10 years, Python has gone from a bleeding-edge or “at your own risk” scientific com‐ puting language to one of the most important languages for data science, machine learning, and general software development in academia and industry.

For data analysis and interactive computing and data visualization, Python will inevi‐ tably draw comparisons with other open source and commercial programming lan‐ guages and tools in wide use, such as R, MATLAB, SAS, Stata, and others. In recent years, Python’s improved support for libraries (such as pandas and scikit-learn) has made it a popular choice for data analysis tasks. Combined with Python’s overall strength for general-purpose software engineering, it is an excellent option as a pri‐ mary language for building data applications.

#### Installation and Setup

Windows

```bash
C:\Users\wesm>python
Python 3.5.2 |Anaconda 4.1.1 (64-bit)| (default, Jul  5 2016, 11:41:13)
[MSC v.1900 64 bit (AMD64)] on win32
>>>
```

Apple (OS X, macOS)
Download the OS X Anaconda installer, which should be named something like Anaconda3-4.1.0-MacOSX-x86_64.pkg. Double-click the .pkg file to run the installer. When the installer runs, it automatically appends the Anaconda executable path to your .bash_profile file. This is located at /Users/$USER/.bash_profile.
To verify everything is working, try launching IPython in the system shell (open the Terminal application to get a command prompt):
```bash
$ ipython
```
To exit the shell, press Ctrl-D or type exit() and press Enter.


GNU/Linux
Linux details will vary a bit depending on your Linux flavor, but here I give details for such distributions as Debian, Ubuntu, CentOS, and Fedora. Setup is similar to OS X with the exception of how Anaconda is installed. The installer is a shell script that must be executed in the terminal. Depending on whether you have a 32-bit or 64-bit system, you will either need to install the x86 (32-bit) or x86_64 (64-bit) installer. You will then have a file named something similar to Anaconda3-4.1.0-Linux-x86_64.sh. To install it, execute this script with bash:
```bash
$ bash Anaconda3-4.1.0-Linux-x86_64.sh
```

After accepting the license, you will be presented with a choice of where to put the Anaconda files. I recommend installing the files in the default location in your home directory—for example, /home/$USER/anaconda (with your username, naturally).
The Anaconda installer may ask if you wish to prepend its bin/ directory to your $PATH variable. If you have any problems after installation, you can do this yourself by modifying your .bashrc (or .zshrc, if you are using the zsh shell) with something akin to:
```bash
export PATH=/home/$USER/anaconda/bin:$PATH
```

After doing this you can either start a new terminal process or execute your .bashrc again with source ~/.bashrc.


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
### 8) [Numpy](https://numpy.org/)
