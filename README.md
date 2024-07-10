**Movie Suggestion-Python**

**Overview**
Using Python script to fetch movie data from IMDb based on user-inputted genres and provide movie suggestions. The script utilizes web scraping to gather data, processes it into a structured format, and allows filtering for further suggestions.

### Dependencies
- `requests`
- `beautifulsoup4`
- `pandas`
- `json`

You can install them using pip:
pip install requests beautifulsoup4 pandas

**Functionality:**
- Constructs the URL for the IMDb search based on the genre.
- Sends a GET request to the constructed URL with a custom User-Agent header.
- Checks the response status and parses the HTML content using BeautifulSoup.
- Extracts movie data from the JSON script embedded in the page.
- Creates a DataFrame with the movie titles and genres.
- Saves the DataFrame to a CSV file (`movies.csv`).
- Reads the CSV file into a DataFrame.
- Filters the DataFrame for movies that contain the specified genre.
- Prints the filtered movies.

**Error Handling:**
- Catches and reports request exceptions.
- Handles missing elements or parsing errors in the HTML content.
- Catches file not found and empty data errors.

### Notes
- The script assumes the structure of IMDb's page remains consistent. Any changes on IMDb's end may require adjustments to the parsing logic.
