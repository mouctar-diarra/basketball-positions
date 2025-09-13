# basketball-positions

This repository uses PyTorch to classify player positions in mens college basketball teams. I created this as a way to explore the PyTorch library and to apply my sports interests with ML.

---
## Webscraping
This Jupyter notebook webscrapes team roster data for NCAA Division I men’s teams to generate player level statistics that are utilized in the main Jupyter notebook (Basketball Positions). Metrics are webscrapped across Division I men's teams over a 20 year period from 2005-2025. Each year of data takes ~2.5-3 hours to properly extract. 

The code can fail to capture some player stats. For example, the player stats csv is missing data in 2021: New Orleans, Brown, Columbia, Cornell, Dartmouth, Harvard, Pennsylvania, Princeton, and Yale. Player stats is also missing St. Francis (NY) Terriers in 2024. Depending on when the code is run, different player stats could not be captured. For completeness, additional webscrapping code can be added to mannually extract data for a specific team and year.

## Data Source
The Jupyter notebook relies on publicly available, web-scraped statistics from:  
[sports-reference.com/cbb](https://www.sports-reference.com/cbb/)  

This includes team roster data for NCAA Division I men’s teams.

## Required Libraries & Modules
This repository contains Jupyter Notebook code that requires the following Python libraries. To run the notebooks successfully, please ensure all dependencies are installed.
For users with a standard Anaconda setup, most packages like `pandas`, `numpy`, `seaborn`, `matplotlib`, and `time` are included by default.  
For packages not included by default, you can install them using `pip` in a terminal or directly in a Jupyter Notebook cell:

* `pip install torch`
* `pip install torchsummary`
* `pip install itables`
* `pip install beautifulsoup4`
