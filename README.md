# MovieReleaseAnalysis
COMP 370 final project
# COMP 370 Project 2: Movie Release Analysis

## Overview
Our team has been hired by a media company to analyze news reporting surrounding the recently released movie **Smile 2** and 14 other movies. This analysis aims to understand:

1. The main topics or aspects of the movies covered in news articles.
2. The extent of media coverage each movie received relative to others released around the same time.

## Goals
- Identify the key topics discussed in articles.
- Compare the volume of coverage for each movie.

## Analysis Details
### Data Collection
- **API Used**: We chose **newscatcherapi** over **NewsAPI.org** due to quota limitations.
- **Number of Articles**: Collected 500+ articles, ensuring an unbiased approach to coverage volume across the movies.
- **Language**: All articles are filtered to be in English.

### Movie List for Analysis
- **Primary Movie**: Smile 2
- **Comparison Movies**:
  - Terrifier 3
  - Beetlejuice Beetlejuice
  - Caddo Lake
  - Venom: The Last Dance
  - Alien: Romulus
  - Conclave
  - The Silent Hour
  - We Live in Time
  - Bookworm
  - Don’t Move
  - Your Monster
  - The Stoic
  - Die Alone
  - Time Cut

### Methodology
1. **Topic Identification**:
   - Conducted open coding on 200 articles using only the title and opening of each article.
   - Developed 3-8 main topics and categorized each article into one topic.

2. **Annotation**:
   - Manually annotated the complete set of 500 articles.

3. **Characterization**:
   - Computed the 10 words with the highest tf-idf scores for each topic. Used the entire dataset of 500+ posts to calculate inverse document frequency.

## Project Structure
```
project2-movie-analysis/
|-- data/
|   |-- raw_articles.csv
|   |-- annotated_articles.csv
|
|-- scripts/
|   |-- data_collection.py
|   |-- data_preprocessing.py
|   |-- topic_analysis.py
|   |-- tfidf_analysis.py
|
|-- results/
|   |-- topic_summary.txt
|   |-- coverage_comparison.csv
|
|-- README.md
```

