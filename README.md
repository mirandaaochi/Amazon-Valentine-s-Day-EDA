# 2024 Amazon Best Sellers: Top Valentine Gifts - Exploratory Data Analysis

## Executive Summary

This exploratory data analysis project was suggested by Jess Ramos through her Substack.

Dataset: [2024 Amazon Best Sellers: Top Valentine Gifts](https://www.kaggle.com/datasets/kanchana1990/2024-amazon-best-sellers-top-valentine-gifts?utm_source=substack&utm_medium=email)

Using SQL, I pulled information from the dataset to identify answers to the following questions regarding Valentine’s Day shopping trends on Amazon:
  * Which products and brands have the best & worst reviews? Why do you think this is?
  * What brands are on the bestseller list most often?
  * Are there any trends between prices and ratings?
  * Which products are above average for 5-star ratings?

## Business Problems
The goal of this EDA is to identify answers to the following questions regarding Valentine’s Day shopping trends on Amazon:
  * Which products and brands have the best & worst reviews? Why do you think this is?
  * What brands are on the bestseller list most often?
  * Are there any trends between prices and ratings?
  * Which products are above average for 5-star ratings?

## Methodology

1. Import dataset to SQL (pgAdmin). Clean the data by dropping or filling null values, depending on their location.

2. Perform SQL queries to identify answers to the business questions.

## Skills

SQL: filters, aggregate functions (MIN(), MAX(), COUNT(), SUM(), AVG(), STDDEV())

## Results

**Which products and brands have the best & worst reviews? Why do you think this is?**

For our analysis, we chose the top products with more than 5 reviews. The top 11 products with the best reviews had 5 or less reviews, all of which were 5-stars. This led their 5-star percentages to be 100%, but few high reviews does not always mean a good product.

Brands were ranked by proportion of 5-star or 3-star reviews regardless of the number of products they have on the Bestseller List or the total number of reviews.

*Products with the Best Reviews*

1. Red Forever Preserved Roses in Heart Shape Gift Box - Roseshy ($49.99)
    * Flowers are a classic Valentine’s day gift.
2. LEGO Icons Wildflower Bouquet Set - Artificial Flowers with Poppies and Lavender ($47.99)
    * LEGOs are a fun activity for adults and children!
3. Cheerin Valentines Day Card with Envelope ($6.99)
    * Everyone loves a good card.
4. GIFTINBOX 28 Pack Valentines Day Gifts for Kids Classroom ($21.99)
    * Valentine’s Day card exchanges are the staple of any Valentine’s Day for children.
5. LEGO Icons Flower Bouquet Building Set - Artificial Flowers with Roses ($47.99)

*Products with the Worst Reviews*

1. Limited Edition M and M’s Milk Chocolate Bark, Valentine’s Day Candy Gift Bag, 5 Ounces ($11.20)
    * Chocolates were not worth the price.
2. Dunkin' Chocolates Heart Box Valentine's Day Gift ($13.99)
3. HAMIMOS Flower Building Blocks with Valentines Cards for Kids Classroom School & Stickers ($14.99)
    * These did not come with instructions. 
4. Asddage Valentines Rose Flowers Birthday Gifts for Women ($7.99)
    * This looks as cheap as it costs.
5. JOYIN 28 Packs Valentine's Day Gift Cards with Flashing LED Bracelets ($22.99)
    * These were missing parts or the LEDs came not working.

*Brands with the Best Reviews*

* Jetrvat
* Weflye
* FINGOOO
* SpringFlower
* Ithmahco

These brands all have 1-5 products.

*Brands with the Worst Reviews*

* Morris National Inc
* Frankford
* HAMIMOS
* Asddage
* BUNNY • JAMES •

These brands all have 1-2 products, which appeared on our worst reviewed products list.

**What brands are on the bestseller list most often?**

Brands were ranked by product's positioning data on Amazon's category pages.

1. Starburst
2. LUCKOR
3. BodyRefresh
4. CRAVEBOX
5. Peacable Kingdom
6. Zalik
7. STUNFASSOO
8. Jinsome
9. LEGO
10. BFJLIFE

**Are there any trends between prices and ratings?**

There are 82 different “price groups” that range in the number of products they contain.
  * The $19.99 group (8 products) has the highest reviews.
  * The $9.99 group has the most reviews (and the most products).

The second best reviewed product is priced at $49.49 with 113 reviews.
  * The first is priced at $3.79 (with one review).

The worst reviewed product is priced at $12.50.

Overall, we cannot necessarily conclude that there are any trends between prices and ratings.

**Which products are above average for 5-star ratings?**

Average Percentage of Ratings:
  * 3 Stars - 5%
  * 4 Stars - 10.5%
  * 5 Stars - 76.8%

These products are on Bestsellers List, so it makes sense that the majority of ratings are 5 stars.

182 products have more than the average 5 star percentage.

Examples:
  * Red Forever Preserved Roses in Heart Shape Gift Box - Roseshy ($49.99)
  * LEGO Icons Wildflower Bouquet Set - Artificial Flowers with Poppies and Lavender ($47.99)
  * Cheerin Valentines Day Card with Envelope ($6.99)
  * GIFTINBOX 28 Pack Valentines Day Gifts for Kids Classroom ($21.99)
  * LEGO Icons Flower Bouquet Building Set - Artificial Flowers with Roses ($47.99)

## Next Steps

1. Measure legitimacy of reviews and adjust analysis.

2. Continue exploring the dataset to reveal additional trends or findings.

3. Build visualizations in Tableau as needed.


