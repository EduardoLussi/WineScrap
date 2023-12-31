# Uncorking the Data: Building a Wine Dataset via Web Scraping

The Wine Game is a project focused on creating Non-Fungible Tokens (NFTs) for individuals' prized wine cork collections. The concept revolves around enabling wine bottle owners to mint an NFT at the very moment they uncork their bottle, resulting in a virtual representation of a cherished wine cork. However, the project hinges on acquiring an extensive dataset of existing wine bottles to accurately match user-owned wines and generate these unique tokens. Unfortunately, such a dataset remains elusive, with existing wine datasets predominantly confined to specific wine attributes or originating from a single website. In response, this paper is a case study of the development of a web scraping method to gather wine bottle data from diverse wine sales websites. Different sources are used in the crawling process and a technique for merging data is also developed.

## Wine Attributes

The essential attributes obtained from the wine listings encompass the following:

- Color: Red, white, rosé, and more.
- Grape Variety: Including Pinot Noir, Cabernet Sauvignon, Vernaccia, and others.
- Region: Covering country, wine region, and wine subregions.
- Price: Displayed in either dollars (\$) or euros (€).
- Vintage: The year of production.
- Ratings: Comprising evaluations from sources such as James Suckling, Jeb Dennuck, and others.
- Size: The bottle's volume.
- Producer: The wine's manufacturer or vineyard.
- Name: The product's specific title.
- Image: The link for an image of the wine.

## Data Sources

We draw from four distinct data sources for this purpose:


- [wine.com](wine.com): The world's largest wine store, boasting nearly 500 thousand wines, wine.com provides a good categorization and ratings information. However, the data on this website lacks a consistent structure, necessitating category-based searches to populate wine attributes.
- [Astorwines](astorwines): With a selection of over 5 thousand wines, Astorwines offers well-organized information. Furthermore, it consistently provides a single image for each wine. Nevertheless, Astorwines faces the difficulty of distinguishing between producer and wine name.
- [Bottlerocket](bottlerocket): This source also boasts organized information and includes valuable review data. 
- [Italian Wine Merchants](italianWineMerchants): Focusing on fine and rare wines, this website stands out for its good categorization.