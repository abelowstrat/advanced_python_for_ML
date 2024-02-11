# AI-supported process monitoring system

Welcome to our Python project! We developed an AI-supported process monitoring system for mechanical engineering as part of a university project. This repository is designed to address advanced data processing tasks using an object-oriented approach for flexibility and scalability. Our project structure is carefully organized to facilitate development, testing, and deployment of machine learning models aimed at signal processing and feature extraction.

## Project Structure

The project is organized into several directories, each serving a specific purpose:

- `modules/`: Contains Python modules for data loading, signal preprocessing, feature extraction, model training, and evaluation.
  - `data_loader/`: For loading data from various sources.
  - `signal_preprocessor/`: Functions for signal preprocessing (filtering, noise reduction).
  - `feature_extractor/`: Extracts features from the preprocessed signals.
  - `learner/`: Algorithms and methods for training machine learning models.
  - `evaluator/`: Functions for evaluating and assessing the trained models.
- `scripts/`: Scripts for specific tasks like data exploration, data extraction, loading experiment data, feature engineering, and model training & evaluation.
- `test/`: Contains test scripts to verify the functionalities of different modules.
- `.data/`: Directory for storing datasets and intermediate results.
- `env/`: Holds the environment configurations required for the project's execution.
- `artifacts/`: Stores results such as plots and model files.
- `config.json`: Configuration file to control various aspects of the project.
- `LICENSE`: Defines the usage rights and restrictions for the project.
- `.gitignore`: Specifies intentionally untracked files to ignore.
- `requirements.txt`: Lists all Python libraries and packages needed.

## Getting Started

### Prerequisites

Ensure you have Python 3.x installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

Before getting started with this project, make sure you have the following Python packages and tools installed:

- [matplotlib](https://matplotlib.org/) (Version 3.8.2)
- [matplotlib-inline](https://pypi.org/project/matplotlib-inline/) (Version 0.1.6)
- [numpy](https://numpy.org/) (Version 1.26.3)
- [pandas](https://pandas.pydata.org/) (Version 2.1.4)
- [scikit-learn](https://scikit-learn.org/stable/) (Version 1.3.2)
- [scipy](https://www.scipy.org/) (Version 1.11.4)
- [seaborn](https://seaborn.pydata.org/) (Version 0.13.1)
- [statsmodels](https://www.statsmodels.org/stable/index.html) (Version not specified)
- [pathlib](https://docs.python.org/3/library/pathlib.html) (Version not specified)
- [tsfresh](https://tsfresh.readthedocs.io/en/latest/) (Version 0.20.2)
- [pytest](https://docs.pytest.org/en/latest/) (Version 8.0.0)

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/link/to/repo
   ```
2. Navigate to the project directory:
   ```
   cd hsa_python_advanced
   ```
3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

### Usage

To run the main script and execute the entire pipeline, simply run:
```
python main.py
```

For executing specific tasks, navigate to the `scripts/` directory and run the desired script. For example:
```
python scripts/data_exploration.py
```

## Configuration (`config.json`)

The `config.json` file plays a crucial role in defining the paths to datasets and specifying algorithms used in the project. Here's a breakdown:

### Experiments

Datasets are organized by experiments, each containing measurements with their respective formats. Adjust the paths as needed when working with your own data.

- Experiment 1-3: Data in `.tsv` and `.csv` formats.
- Experiment 4: Data serialized in `.pkl` format.

Paths are relative to the `.data/` directory, ensuring organized and accessible data management.

### Algorithms

Machine learning algorithms configured for use:

- **Random Forest**: With 1000 estimators and a fixed random state for reproducibility.
- **Decision Tree**: Configured with a maximum depth to prevent overfitting.
- **K-Nearest Neighbors (KNN)**: Set with 3 neighbors for classification.

This structure allows for flexible experimentation with different machine learning strategies and data preprocessing methods.

Please note that this project is configured to be used on univariate time series.

### Testing

To ensure the reliability of our modules, run the test scripts located in the `test/` directory:
```
python -m unittest discover test
```

## Contributing

Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Acknowledgments

Thanks to all project members and contributors who have invested their efforts in the development of this project.
