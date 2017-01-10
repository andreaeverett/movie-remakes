### Explaining and the popularity of movie remakes through the original

A blog post describing the project and presenting some of the results is available at https://andreaeverett.github.io/blog/Film_Remakes/.

##### Code summary:

The code for this project is contained in 3 Jupyter notebooks:

1. '1_movie_remake_pairs': This file uses BeautifulSoup to collect a list of paired films -- one remake and one original -- from Wikipedia. It saves them in a CSV file, creating a single entry for each film to ease further data collection.

2. '2_get_omdb_data': This file uses the OMDB API to collect ratings and other information about the film-list previously compiled from Wikipedia. It also cleans these data and uses them to generate new features appropriate for statistical analysis. Finally, it combines the films back into a list of paired originals and remakes, and generates several more features based on the relationship between the two.

3. '3_analysis': This file analyzes the original-remake movie pairs data prepared in the two previous notebooks. It focuses on linear regression and random forests, using cross-validation for feature selection.

##### Other files:

1. 'data_files': This folder contains all of the data files generated in the 3 notebooks, including the 2 html pages from Wikipedia.

2. 'figures': This folder contains figures produced and saved in the final notebook ('3_analysis') and shown in the above-referenced blog post.
