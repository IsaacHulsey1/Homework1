---
output:
  html_document:
    keep_md: true
---
# Question 1
## Isaac Hulsey idh285










### I'm interested in whether or not there's an airport you don't want your flight from Austin to come from in regards to average delay time. So, first I created a simple scatterplot between airport of origin and delay time to see if any trends existed.

![](Airport_files/figure-html/unnamed-chunk-4-1.png)<!-- -->

### It appears that a few airports have longer average delay times than others. So, I calculated the average delay time in minutes for every airport of origin, and I created a bar graph to visualize average delay time in Austin from airport of origin in descending order.




![](Airport_files/figure-html/unnamed-chunk-6-1.png)<!-- -->

### It looks like you don't want your flight to originate from Knoxville (TYS), Oklahoma City (OKC), or Philidelphia (PHL) as those have an average delay time between 80 and 95 minutes when flying to the Austin airport.

# Question 2

## For Subclass 350


### For starters let's take a look at what the data looks like for the 350 subclass.


![](Airport_files/figure-html/unnamed-chunk-8-1.png)<!-- -->



![](Airport_files/figure-html/unnamed-chunk-10-1.png)<!-- -->





### What we see in this graph shows that as k increases, rmse of the out of sample prediction decreases. What I suspect is going on is that most of the data in this set for the 550 subclass is for cars with less than 50,000 miles. Also, the data in the range of 0 to 50,000 miles doesn't have an obvious trend in the price range (excluding the new cars have a higher price). So, the best prediction in kmeans for the price of the car given how many miles driven it has in the 550 subclass might end up being the sample average. 

# Now for Subclass 65AMG

### Starting with the plot of the data
![](Airport_files/figure-html/unnamed-chunk-12-1.png)<!-- -->


### Contrast this scatterplot of mileage against price for 65AMG with the 550 with the corresponding scatterplot for the 550 subclass. There is a trend that we can see. The higher the mileage, the loweer the the price tends to be. There isn't a "clump" of data in this data.



![](Airport_files/figure-html/unnamed-chunk-14-1.png)<!-- -->

### Just as expected, there does seem to be a cutoff for optimal value of k for the out of sample RMSE prediction for the 65AMG model. Let's graph this again, but this time "zoomed in" on values of k between 150-220



![](Airport_files/figure-html/unnamed-chunk-16-1.png)<!-- -->

### The optimal K tends to be somewhere between 200-220 for the 65AMG Subclass.It just depends on what data ends up being in the test set.
