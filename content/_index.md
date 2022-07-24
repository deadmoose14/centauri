---
title: ""
date: 2022-07-23T17:51:55-04:00
draft: false
---
# Posts
Important updates will go here, including quick links to each respective classes notes[^1]/assignments[^2] issued for the day. 


Period  | Class | Links
--------|-------|--------
2       | TBD   | TBD 
3       | TBD   | TBD 
4       | TBD   | TBD 
5       | TBD   | TBD 
6       | TBD   | TBD 
7       | TBD   | TBD 

Blockquotes 
> With great power comes great responsibility


Here is a `code` block. 

```R
stirling <- function(z) sqrt(2*pi/z) * (exp(-1)*z)^2

nemes <- function(z) sqrt(2*pi/z) * (exp(-1)*(z+(12*z-(10*z)^-1)^-1))^z

lanczos <- function(z)
{
    if(length(z) > 1)
    {
        sapply(z, lanczos)
    } else 
    {
        g <- 7
        p <- c(0.99999999999980993, 676.5203681218851, -1259.1392167224028,
        771.32342877765313, -176.61502916214059, 12.507343278686905,
        -0.13857109526572012, 9.9843695780195716e-6, 1.5056327351493116e-7)
        z <- as.complex(z)
        if(Re(z) < 0.5)
        {
            pi / (sin(pi*z) * lanczos(1-z))
        } else
        {
            z <- z - 1
            x <- p[1] + sum(p[-1]/seq.int(z+1, z+g+1))
            tt <- z + g + 0.5
            sqrt(2*pi) * tt^(z+0.5) * exp(-tt) * x
        }
    }
}

spouge <- function(z, a=49)
{
    if(length(z) > 1)
    {
        sapply(z, spouge)
    } else 
    {
        z <- z-1
        k <- seq.int(1, a-1)
        ck <- rep(c(1,-1), len=a-1 / factorial(k-1) * (a-k)^(k-0.5) * exp(a-k)
        (z + a)^(z+0.5) * exp(-z-a) * (sqrt(2*pi) + sum(ck/(z+k)))
    }
}
```

<!-- ![Example](ex.png) -->

# References
[^1]: Made you look. 
[^2]: Made you look again.
