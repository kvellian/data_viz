This project aims to explore what the average single-family home in Texas could look like through data visualization.

Data Bias:
- According to the source, this dataset features “a curated selection of 500 property listings. It encompasses a wide array of properties, reflecting the diverse real estate landscape across Texas”, which indicates that there is some bias with the data selection.

## Data Exploration

## Data Cleaning

Collaboration with our team, GraphGurus: 
- Performed by Francisco Lozano: KNN Imputation to clean missing square footage, # of stories, and year built.
- Performed by Ken Vellian: Extract address information, through regular expressions, from the URL column to create the new street address, city, state, and zip columns. Extract square footage and acre size, through regular expressions, from the text column and fill in missing square footage values.

## Initial Analysis

Using this bar plot, to count properties by type, we can confirm our assumption about the large presence of single-family homes in the dataset, with 400 listings. This explanatory visualization displays the sums of each type at the top of the bar to inform the reader of the exact count, and the size of the bars allows us to visually gauge each type's impact on the dataset. Exploring this property type further might provide great insights due to its large significance. It will allow us to make reasonable estimations when diving deeper.

<img src="/assets/img/count_bar_plot.png" alt="Count Bar Plot image">

## Average Single-Family Home
