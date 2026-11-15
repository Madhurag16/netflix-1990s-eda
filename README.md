
# Netflix 1990s Movies: Exploratory Data Analysis

Exploratory analysis of Netflix movies released in the 1990s, framed as research for a production company that specializes in nostalgic styles.

## Questions

1. What was the most frequent movie duration in the 1990s?
2. How many short action movies (under 90 minutes) were released in the 1990s?

## Dataset

`netflix_data.csv` contains Netflix titles with these columns: `show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `duration` (minutes), `description`, `genre`.

Source: DataCamp project dataset.

## Approach

- Filtered to `type == "Movie"` and `release_year` from 1990 to 1999
- Plotted a histogram of durations to see the distribution
- Picked the approximate most frequent duration from the histogram peak
- Filtered to the Action genre and counted movies under 90 minutes

## Key Findings

- **Most frequent duration:** about 100 minutes
- **Short action movies (1990s):** [X]

### Distribution of 1990s Movie Durations

![Distribution of 1990s movie durations](duration_histogram.png)

- Most 1990s movies on Netflix run between 90 and 120 minutes.
- A smaller second cluster appears around 150 to 190 minutes, likely epics and longer dramas.
- A handful of very short titles sit near 30 minutes.

## Tools

Python, pandas, matplotlib, Jupyter Notebook

## Files

- `notebook.ipynb`: full analysis with code and charts
- `duration_histogram.png`: duration distribution chart
- `README.md`: project overview

## How to Run

```bash
pip install pandas matplotlib jupyter
jupyter notebook notebook.ipynb
```
