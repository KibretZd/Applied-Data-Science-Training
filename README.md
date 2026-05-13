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