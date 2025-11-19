project:
  name: "Fitness Data Analysis"
  description: >
    A Jupyter Notebook project that analyzes a random fitness dataset.
    It covers data loading, exploration, cleaning, timestamp transformation,
    feature engineering, and visualizations using Python.

libraries_used:
  - pandas
  - numpy
  - datetime
  - matplotlib
  - plotly

dataset:
  file: "random_fitness_dataset.csv"
  operations:
    - load_dataset:
        code: "fitness_df = pd.read_csv('random_fitness_dataset.csv')"
    - preview_rows: "fitness_df.head(10)"

data_exploration:
  steps:
    - structure_check: "fitness_df.info()"
    - statistical_summary: "fitness_df.describe()"
    - null_check_any: "fitness_df.isna().values.any()"
    - null_check_count: "fitness_df.isnull().sum()"

timestamp_cleaning:
  convert_timestamp:
    description: "Converts 'time_stamp' column into datetime objects"
    code: "fitness_df['time_stamp'] = pd.to_datetime(fitness_df['time_stamp'])"

feature_engineering:
  new_features:
    - date:
        description: "Extracts date part from timestamp"
        code: "fitness_df['date'] = fitness_df['time_stamp'].dt.date"
    - month:
        description: "Extracts month name"
        code: "fitness_df['month'] = fitness_df['time_stamp'].dt.month_name()"
    - day:
        description: "Extracts day name"
        code: "fitness_df['day'] = fitness_df['time_stamp'].dt.day_name()"
    - hour:
        description: "Extracts hour of the day"
        code: "fitness_df['hour'] = fitness_df['time_stamp'].dt.hour"

visualization:
  tools:
    - matplotlib
    - plotly
  purpose: >
    Used for generating static and interactive charts to explore
    time-based fitness patterns.

project_structure:
  - random_fitness_dataset.csv
  - fitness_analysis.ipynb
  - README.md

how_to_run:
  install_dependencies: "pip install pandas numpy matplotlib plotly"
  run_notebook: "jupyter notebook"

notes:
  - "Dataset appears synthetic and used for learning."
  - "Notebook teaches data cleaning and timestamp manipulation."
  - "Can be extended with correlations, trend analysis, or forecasting."

