# Amazon_Vine_Analysis

Using Colab, Postgresql and ETL techniques to analyze large data sets. 

# Core Questions

## Total Reviews
One of the key questions asked about our data sets refrains to the number of reviews posted by both users and non-vine users.  After breaking down the data we are able to see within the dataset that I had selected there were 613 total reviews from vine users; while non-vine users equated to just shy of 65K(64,968).

![ImageOfVineTotalReviews](https://github.com/Gkmb2390/Amazon_Vine_Analysis/blob/main/yes_total_reviews.png)
![ImageOfNonVineTotalReviews](https://github.com/Gkmb2390/Amazon_Vine_Analysis/blob/main/no'_total_reviews.png)


## Total 5 Star Reviews 
The total number of 5-star reviews registered to vine users, as seen below came in at 222.  
![ImageOfVine5Reviews](https://github.com/Gkmb2390/Amazon_Vine_Analysis/blob/main/yes_5_star.png)

The number of non-vine 5-star reviews came in at a total of 30,543.
![ImageOfNonVine5Reviews](https://github.com/Gkmb2390/Amazon_Vine_Analysis/blob/main/no_5_star.png)


## Total 5 Star Percentages
We can now calculate the percentage of 5-star reviews from vine users, by using the 2 elements we previousl created for total review and 5-star reviews.  Ultimately this results in a .3621, which when converted to a percentage would equate to 36.21% or 36% rounded. 
![ImageOfVine5Precent](https://github.com/Gkmb2390/Amazon_Vine_Analysis/blob/main/yes_5_star_percent.png)

Using the same principals, applied to the non-vine 5-star percentage as .47 or 47%.
![ImageOfNonVine5Precent](https://github.com/Gkmb2390/Amazon_Vine_Analysis/blob/main/no_5_star_percent.png)


# Summary

One may assume that positivity bias would inherently exist in the vine reviews.  Since They are being incentivized, to some extent, to produce reviews.  However, when we compare the results of the vine users vs the non vine reviews we see a lower percentage of 5-star reviews by comparison.  Obviously we would need to conduct a more through and rigourous statistcal review of the data we have aggregated. But if one were attempting to prove a positivity bias among vine users; one would assume that the vine users would have, at least a minimally higher overall greater percentage of 5-star reviews.  Givent that the percentage is lower we are left to conclude that the positivity bias is not present among vine-users.  

Another analysis that we could use to interpret the data is to consider the number of reviews by those that actually purchased the products.  The verified_purchase column amongst, our dataset was a mixed bag among the non-vine users, as well as the vine users.  If we wanted to confirm any kinds of bias amongst the results, we should probably start by filtering to those whom have purchased and utilized the products in question.