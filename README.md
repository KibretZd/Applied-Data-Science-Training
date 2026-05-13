# Applied-Data-Science-Training
The Applied Data Science Training is organized by College of Informatics held from May 13-15, 2026.
Mastery of :
. Data Analysis Pipeline from Data Loading to interpret and communicaing insights for better decision making.
. ML to analyze research data, build predictive models, and apply data-driven decision making in academic and professional contexts.

Data Analysis:
 . Data-driven fields or subfields: Data Science, Data Analytics, data analysis.
 . it is a systematic process of collecting, cleaning, transforming and interpreting data to find useful insights and support decision making.

Key stages of Data Analysis Pipeline:
1. Problem Definition
    - clearly state the RQ or hypothesis
    - align Objective with computing goals
2. Data Acquisition
    - sources: dbs, APIs, sensors
3. EDA
    - use statistical summaries and visualizations
    - identify correlations
4. Data Cleaning and prepocessing
    -   handle missing values, duplicates and inconsistencies
    - normaliza, encode and engineer features
5. Modeling
6. Evaluation
    - metrics: Accuracy, F1-Score, RMSE, AUC depending on the task
    - ensure generalizations to unseen data
7. Deploy and Monitoring

## Data Loadindg and EDA
    - Dataset Loading
    - Explanatory Data Analysis
    - View and Understand the Dataset
        . Statistical Summaries
        . Data Quality Assessment
Types of Dataset
1. By Structure
    a. Structured

2. By Content or Type
    a. qualitative
    b. quantitatie
    c. spacial
    d. Multimedia

3. By File Format
    - Text-based
    - Binary/columnar
    - specialized - dommain specifice formats (E.g DICOM for medical images, Shapefiles for GIS)
4. By Time Dependency
    - Static
    - Dynamic/Temporal
    - Streaming - generated, transmittedd, and processed in continously in real-time

### Data Loading and Injestion
    The process of transferring raw data from persistent storage into a computational container
    Sources:
    - File systems
    - Data base Systems
    - Remote Services cloud storage like S3, GCS...
    - Curatedd Repositories - Integrated loaders (e.g scikit-learn, Hugging Face Hub, Kaggle, UCI, OpenML)
    Computational Containers:
        - Tabular Structures
        - N-Dimensional Arrays

### EDA
    - Feature Analysis
    It is the process of explorig and evaluating dataset features to understand their characterstics, r/nships, importance, and impact on model performance
    Common acctivities in feature analysis include:
        . statistical summary
        corelation analysis
        distribution analysis
        feature importance evaluation
        Dimensionality analysis
        dulicacy detection
        -visualization of feature behavior
    - Data Visualization

#### Types of Feature analysis
    1 Univariate analysis - single vairiable
    2. Bivariate analysis - two variables
     -Techiniques
        . Num vs Num
        . Cat vs Num
        . Cat vs Cat
    3. Multivariate Analysis - high dimentional
        - Heatmaps, PCA

#### Correlation
. measures the stringth and direction of linear r/ship between two numeric features
. values range between -1 tot 1:
    - +1 - Perfect +ve correlation
    - 0 - no linear r/ship
    - -1 - Perfect -ve correlation
    - Techniques:
        - use Heatmap and correlation matrix

    Multicolinearity is a situation in which two or more independent features in a dataset are highly correlated with each other
     . VIF (Variance Inflation Factor) is the most commonly used to detect multicolinearity.
        - a VIF >5 or 10 is considered problematic
        - 1 - no multicollinearity
        - >10 seriously multicollineaarity
#### Data Visualization
Tools

    - matplotlib - basic ploting, highly customizable
    - Seaborn - built on matplotlib, easy statistical plots (histogram, heatmaps, boxplots)
    - plotly - interactive plots that you can zoom, pan and hover over.

Types of Plots and used

    - histplot - Distribution
    - boxplot - spread
    - scatter - relationship between two variables
    - heatmap - correlation

Identify unique categoris of categorical features
    . df.nunique() 
        - Count number of distinct elements in specified axis.
        - Return Series with number of distinct elements. Can ignore NaN values.

    . df.unique() - uniques are returned in order of appearance. Hash table-based unique, therefore does NOT sort.
        - returns all distinict values in a column
        - it is also used to identify unique categories of categorical feature.
        ```python
        df['property_type'].unique()


### Data Spliting (Train /Validation /Test)

To get honest, unbiased estimate of how well your model perform on new, unseen data, split your dataset into independent subsets

    - Training set: to train the model
    - Validation set: to tune hyperparameters
    - Test set - used for only final evaluation

Common Spliting Options

    . Train/Test split
        - Simple and faster
        - Commonly used for small projects and baseline models
        - Example: 80% Train, 20% Test

    . Train/Validation/Test Split
        - More reliable for model tuninng and selection
        - commonly used in real-world ML workflows
        - Example: 60% Train, 20% Validation, 20% Test

    . before preprocessing (imputation, scaling and encoding) to avoid data leaakage
    . use stratify = y for classification task to preserve class distribution
    . use a fixed random_state (e.g 42) for reproducibility
