# GitHub Topic Scraper By Om Anand JHA (TSI)

A Python package for scraping GitHub topics and their top repositories.

## Installation

```bash
pip install github-topic-scraper
```

## Usage

```python
from github_topic_scraper import GitHubTopicScraper

# Initialize the scraper
scraper = GitHubTopicScraper()

# Scrape topics and repositories
topics_df = scraper.scrape_all()

# Access the scraped data
topics_df.head()
```

## Features

- Scrapes GitHub topics and their descriptions
- Collects top repositories for each topic
- Saves data to CSV files
- Includes error handling and progress tracking
- Configurable output directory

## Requirements

- Python 3.7+
- requests
- pandas
- beautifulsoup4

## Troubleshooting Installation

### 1. Setting up Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 2. Installing Dependencies

```bash
# Make sure your virtual environment is activated
pip install requests pandas beautifulsoup4
```

### 3. Installing Package in Development Mode

```bash
# Make sure you're in the github_topic_scraper directory
pip install -e .
```

### 4. Verifying Installation

```bash
# Start Python interpreter
python

# Try importing the package
>>> from github_topic_scraper import GitHubTopicScraper
# If no error appears, the package is installed correctly
>>> exit()
```

### 5. Running Sample Code

```python
from github_topic_scraper import GitHubTopicScraper

scraper = GitHubTopicScraper(output_dir="sample")
topics_df = scraper.scrape_all()
```

If files aren't being generated:
1. Verify your virtual environment is activated (you should see `(venv)` in your terminal)
2. Confirm all dependencies are installed: `pip list`
3. Check you have write permissions in the output directory
4. Ensure you're running the code from the correct directory

## Common Issues

1. **ImportError**: Make sure all dependencies are installed in your virtual environment
2. **Permission Error**: Check write permissions in your output directory
3. **ModuleNotFoundError**: Verify the package is installed correctly

For additional help, please open an issue on GitHub.
