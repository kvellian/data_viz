# Visualizing Texas Real Estate Trends 2024: 500 Listings 🏠

- [Kaggle Data Source](https://www.kaggle.com/datasets/kanchana1990/texas-real-estate-trends-2024-500-listings/data)

This project aims to explore what the average single-family home in Texas could look like through data visualization.

Data Bias:
- According to the source, this dataset features “a curated selection of 500 property listings. It encompasses a wide array of properties, reflecting the diverse real estate landscape across Texas”, which indicates that there is some bias with the data selection.

## Data Exploration

- Original data: 501 rows, 14 columns.

| Category    | Field             | Description                                       |
|-------------|-------------------|---------------------------------------------------|
| Categorical | status            | Current status of listing - all are currently for sale |
|             | sub_type          | Sub Category of property type, such as “condo” or “townhouse” |
|             | text              | Text description narrative used in listing, descriptor of characteristics of property |
|             | type              | General type of property                          |
|             | year_built        | Year the property was constructed                 |
|             | url               | Realtor.com page for listing                      |
|             | id                | Unique Numerical Listing ID                       |
| Numerical   | listPrice         | The asking price                                  |
|             | baths             | Total number of baths in the house                |
|             | baths_full        | Number of full bathrooms                          |
|             | baths_full_calc   | Calculated number of full bathrooms               |
|             | beds              | Number of Bedrooms                                |
|             | sqft              | Square footage of property                        |
|             | stories           | Number of stories in property                     |
| Geographical (created through URL column extraction)| street_address    | The street address of the property listing        |
|             | city              | City of listing                                   |
|             | state             | State of listing (Texas)                          |
|             | zip               | Zip code of listing                               |

## Data Cleaning

Collaboration with our team, GraphGurus: 
- Performed by Francisco Lozano: KNN Imputation to clean missing square footage, # of stories, and year built.
- Performed by Ken Vellian: Extract address information, through regular expressions, from the URL column to create the new street address, city, state, and zip columns. Extract square footage and acre size, through regular expressions, from the text column and fill in missing square footage values.

## Initial Analysis

Using this bar plot, to count properties by type, we can confirm our assumption about the large presence of single-family homes in the dataset, with 400 listings. This explanatory visualization displays the sums of each type at the top of the bar to inform the reader of the exact count, and the size of the bars allows us to visually gauge each type's impact on the dataset. Exploring this property type further might provide great insights due to its large significance. It will allow us to make reasonable estimations when diving deeper.



<img src="assets/img/count_bar_plot.png" alt="count_bar_plot">

<img src="assets/img/sqft_dist.png" alt="sqft_dist">

<img src="assets/img/price_dist.png" alt="price_dist">

<img src="assets/img/bed_vs_bath_heatmap.png" alt="bed_vs_bath_heatmap">




