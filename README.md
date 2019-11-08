# Data 512 Final Project

## Project:

Evaluation Bias towards favored writers in long-time readers

## Project Goals & Motivation:

To quantifiably prove assessment and evaluation biases amongst long-time readers of authors using the [Amazon Review Dataset](https://nijianmo.github.io/amazon/index.html). The project is intented to produce principled, verifiable research that aims to quantify human biases in a (very narrow) space, which are, book reviews across the amazon and kindle platform.


__Unknowns and dependencies__:
Several unknowns exist at this moment.

## Data Source

The partial [Amazon Review Dataset](https://nijianmo.github.io/amazon/index.html) (Jianmo Ni et al.<sup>[1]</sup>) is the key data source for the project. 

The data is split into two parts:
1. The Review Data: The key raw fields for the reviews and ratiings
2. The Metadata: Aggregated data, containing additional information about the review

__1. Review Data__:
1. reviewerID - A Unique ID of the reviewer, on amazon.com
2. asin - Unique Product ID
3. reviewerName - Reviewer Name
4. vote - Helpful Votes
5. style - a disctionary of the product metadata, e.g., "Format" is "Hardcover"
6. reviewText - Blob text of the review
7. overall - product rating
8. summary - summary of the review
9. unixReviewTime - time of the review (unix time)
10. reviewTime - time of the review (raw)

__2. Metadata__:
1. asin - ID of the product, e.g. 0000031852
2. title - name of the product
3. feature - bullet-point format features of the product
4. description - description of the product
5. price - price in US dollars (at time of crawl)
6. imUrl - url of the product image
7. related - related products (also bought, also viewed, bought together, buy after viewing)
8. salesRank - sales rank information
9. brand - brand name
10. categories - list of categories the product belongs to
11. tech1 - the first technical detail table of the product
12. tech2 - the second technical detail table of the product
13. similar - similar product table

## License

The partial [Amazon review dataset](https://nijianmo.github.io/amazon/index.html#citation)<sup>[1]</sup> is openly available for use and experimentation. The complete dataset can be accessed upon request from the team. Citation is needed in both cases.

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/nmnshrma/data-512-a1/blob/master/LICENSE) file for details

## Acknowledgments & Citations:

1. Justifying recommendations using distantly-labeled reviews and fined-grained aspects (Data Source)
Jianmo Ni, Jiacheng Li, Julian McAuley
_Empirical Methods in Natural Language Processing (EMNLP), 2019_, [pdf](http://cseweb.ucsd.edu/~jmcauley/pdfs/emnlp19a.pdf)

