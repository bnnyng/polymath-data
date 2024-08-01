This script is designed to scrape all pages associated with Wikipedia's [Category:Fields of mathematics](https://en.wikipedia.org/wiki/Category:Fields_of_mathematics) and its subcategories. To run the script, make a copy of `scrape-wikipedia.ipynb` and ensure that all files in `filtering-lists` are accessible in the Colab session. This folder contains the following text files, in order of appearance in the notebook:

- `wiki-categories-remove.txt` – category names to exclude from scraping; can be customized
- `categories-level1.txt` – highest level of categories corresponding to broad mathematical subfields (e.g., algebra, analysis, number theory); used to interpret URL scraping progress
- `urls-categories-remove.txt` – output from `get_page_urls()` after excluding categories in the remove list

The results of this notebook are saved in `wikipedia-data/wikipedia-docs.txt`, where each line is a paragraph of some page. Running the script also produces [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) with extended metadata and a unique ID for each paragraph.
