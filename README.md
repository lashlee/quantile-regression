README
================
John Lashlee
2/24/2019

Purpose
-------

The purpose of this repo is to be an example of quantile regression for my colleague. It heavily lifts from the following two sources:

-   Ford, Clay. "University of Virginia Library Research Data Services Sciences." *Getting Started with Quantile Regression*, University of Virginia Library, 20 Sept. 2015, data.library.virginia.edu/getting-started-with-quantile-regression/.

-   Brendan-R. "Brendan-r/quantile\_regression." *Quantile Regression with R, JAGS and Stan*, GitHub, 15 Oct. 2015, github.com/brendan-r/quantile\_regression.

Data
----

Here's one thing everybody agrees on: trains are really great! It's just unanimous.

Say your boss is a Regional Manager of a bunch of train stations. You're the Assistant to the Regional Manager. Your trains mostly come on time, but as with anything in life, there is some variability. It really sucks when a train is late, so you want to reduce the train arrival **wait times**. You study your trains and propose an **improvement** that will make them arrive faster. Your **improvement** is targeted at reducing the *90th percentile* of the arrival **wait time**.

There are two **types** of trains in service, *new* trains and *old* trains.

The trains run on three train **platforms**, *main* platform, *south* platform, and *west* platform.

You implemented your improvement on some trains and held it back from others. Now all that's left to prove the value of your improvement is to

-   collect your train arrival **wait time** data,
-   noting
    -   the train **type**,
    -   **platform**,
    -   and whether or not it had the **improvement** active,
-   run and interpret the quantile regression.
