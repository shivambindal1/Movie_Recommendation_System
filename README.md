
# TMDB Movie Recommendation System

## Overview

This project implements a movie recommendation system using the TMDB 5000 credits dataset. It provides personalized movie suggestions based on collaborative filtering and content-based approaches, utilizing information about movie cast, crew, and other attributes.

## Table of Contents

- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Dataset

This system uses the TMDB 5000 credits dataset, which is part of the larger TMDB 5000 movie dataset available on Kaggle. The `tmdb_5000_credit.csv` file contains the following key information:

- `movie_id`: Unique identifier for each movie
- `title`: Movie title
- `cast`: JSON formatted string with cast information
- `crew`: JSON formatted string with crew information

## Features

- Data preprocessing of TMDB credit information
- Feature extraction from cast and crew data
- Collaborative filtering for user-based recommendations
- Content-based recommendations using movie metadata
- Simple command-line interface for interaction

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/tmdb-movie-recommender.git
   cd tmdb-movie-recommender
   ```

2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install required packages:
   ```
   pip install -r requirements.txt
   ```

4. Download the `tmdb_5000_credit.csv` file from Kaggle and place it in the `data/` directory.

## Usage

Run the main script:

```
python src/movie_recommender.py
```

Follow the prompts to input a movie title and receive recommendations.

## Project Structure

```
tmdb-movie-recommender/
│
├── data/
│   └── tmdb_5000_credit.csv
│
├── src/
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── feature_extraction.py
│   ├── collaborative_filtering.py
│   ├── content_based.py
│   └── movie_recommender.py
│
├── tests/
│   ├── __init__.py
│   ├── test_data_preprocessing.py
│   ├── test_feature_extraction.py
│   └── test_recommendations.py
│
├── README.md
├── requirements.txt
└── LICENSE
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- TMDB for providing the dataset
- Kaggle for hosting the dataset
- All contributors to this project
