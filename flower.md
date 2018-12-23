A flower in the wild
================
Amin Yakubu
12/23/2018

Let's start by drawing 50 points on a circle of radius 1. As every (x, y) point should be in the unit circle, it follows that x² + y² = 1.We can get this using the Pythagorean trigonometric identity which states that sin²(θ) + cos²(θ) = 1 for any real number θ.

Remember, circumference of a circle is C=2πr

``` r
t <- seq(0, 2*pi, length.out = 50)
x <- sin(t)
y <- cos(t)
df <- data.frame(t, x, y)

# Make a scatter plot of points in a circle
p <- ggplot(df, aes(x, y))
p + geom_point()
```

![](flower_files/figure-markdown_github/unnamed-chunk-1-1.png)
