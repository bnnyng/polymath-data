# polymath-data

All comments and posts scraped from the [Polymath Project](https://en.wikipedia.org/wiki/Polymath_Project), based on projects listed [here](https://web.archive.org/web/20200328143655/http://michaelnielsen.org/polymath1/index.php?title=Main_Page). Notebooks for web scraping are located in the "code" folder. 

This repository has the following data files:
- `all-project-comments.json` – all Polymath comments up to Polymath16
  - `author`
  - `author-href`
  - `time`
  - `comment-href`
  - `comment-id`
  - `content`
  - `child-ids`
  - `blog`
  - `post-id`
  - `id`
  - `in-reply-to`
  - `in-reply-to-href`
  - `project-id`
  - `content-no-tex`
  - `tex-count`
  - `content-cleaned`
- `all-project-posts.json` – all Polymath main blog posts with each paragraph saved as a separate document
  - `project-id`
  - `post-id`
  - `post-href`
  - `paragraph-idx`
  - `paragraph-content`
  - `id`
  - `content-no-tex`
  - `tex-count`
  - `content-cleaned`
- `wikipedia-docs.txt` – document file where each line is an entire paragraph from some Wikipedia page about math. A [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) with additional metadata and custom IDs can be created using the `scape-wikipedia.ipynb` notebook.
