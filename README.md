# Module 6 Challenge: Movie Data Analysis Project

This project collects movie reviews from The New York Times API and detailed movie information from The Movie Database (TMDB). It combines these sources to analyze trends in movie genres, languages, and production countries, providing practical insights into the film industry.

## Table of Contents

- [Introduction](#introduction)
- [Technology Used](#technologies)
- [How to Setup](#setup)
- [Features](#features)
- [Code Examples](#code-examples)
- [Status](#status)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to create a unified dataset that blends movie reviews with detailed movie metadata. This combined resource is designed for diverse analytical applications, such as assessing sentiments in reviews, tracking genre popularity, and exploring language variations in movies.

## Technology Used

- Python 3.8+
- Pandas
- Requests
- Jupyter Notebook

## How to Setup

To run this project, install the required libraries using:

```bash
pip install pandas requests
```

Ensure you have API keys for both The New York Times and The Movie Database. Store these keys in your environment variables or a .env file for security.

## Features

- Extract and process movie reviews using The New York Times API.
- Gather comprehensive movie information from The Movie Database (TMDB).
- Combine and clean the data into a unified DataFrame.
- Save the consolidated data to a CSV file for additional analysis.
- Offer tools for preliminary data analysis in a Jupyter Notebook.

## Code Examples

As an example, to fetch data from The Movie Database see the code below:

```bash
import requests

def fetch_movie_data(title):
    url = f"https://api.themoviedb.org/3/search/movie?query={title}&api_key={tmdb_api_key}"
    response = requests.get(url)
    return response.json()
```

## Status

The project is currently operational and remains adaptable for further development and enhancement. Upcoming improvements could incorporate more sophisticated data analysis methods and enhanced interactive visualizations.

## Contributing

Contributions to the project are welcome but the author only did this as a class assignment so I won't be maintaining it. 

## License

This project is licensed under the MIT License.
