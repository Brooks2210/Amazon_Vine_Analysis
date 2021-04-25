# Amazon Vine Analysis

## Overview
Amazon has a program called Amazon Vine in which businesses pay a small fee to have their products reviewed. A select group of reviewers are given free products with the stipulation that they provide a written review of that product. Our team has been tasked with analyzing the reviews on Amazon and determining if the Amazon Vine reviewers have a bias in handing out five-star reviews or if their reviews are in line with the rest of the reviews that the products receive from non-compensated reviewers. For our data set we will be looking at the reviews of sneakers sold on amazon. 
### Tools
Google Colab, Amazon AWS, pgAdmin/postgres , and PySpark<br/>
## Results
The first step in our analysis was to clean up the data that was provided. In addition to removing null values and products that did not have a large enough number of reviewers, we also needed to separate the Amazon Vine reviews from the non-vine reviews. Using PySpark to import our data it was just a matter of using various filters and group-bys to structure the data into a useful format and upload into a postgress server. The results of our analysis are below.
![ Percentage_Vine_nonvine](https://github.com/Brooks2210/Amazon_Vine_Analysis/blob/main/Percentage_Vine_nonvine.png)

- A total of 26,993 reviews met our minimum criteria to be analyzed.
- Only 22 of 26,993 were paid Vine reviews. The rest included non-Vine reviews.
- Vine reviewers handed out 5-star reviews 59.09% of the time compared to 53.67% for non-Vine reviewers.
## Summary
In analyzing the data, it does not appear to show a bias towards 5-star reviews by Amazon Vine reviewers. However, it is difficult to gain a complete picture of the review bias with just a small snapshot of the entire process. Additional analysis can be performed in many areas, but our team recommends two starting points.
-	Compare the reviews of Amazon Vine reviewers and non-Vine reviewers on the exact same product. Our analysis only focused on one category and not one specific product.
-	Increase the number of Amazon Vine reviewers. With only 22 Amazon Vine reviews of shoe products, there is too great a risk of not having a large enough sample size to make any type of conclusive argument.  
