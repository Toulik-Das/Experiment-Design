# Experiment-Design

## Types of Study

There are many ways in which data can be collected in order to test or understand the relationship between two variables of interest. These methods can be put into three main bins, based on the amount of control that you hold over the variables in play:</br>

 1.If you have a lot of control over features, then you have an experiment.</br>
 2.If you have no control over the features, then you have an observational study.</br>
 3.If you have some control, then you have a quasi-experiment.</br>
 
While the experiment is the main focus of this course, it's also useful to know about the other types of study so that you can use them in effective ways, especially if an experiment cannot be run.

## Types of Experiment

Most of the time, when you think of an experiment, you think of a between-subjects experiment. In a between-subjects experiment, each unit only participates in, or sees, one of the conditions being used in the experiment. The simplest of these has just two groups or conditions to compare. In one group, we have either no manipulation, or maintenance of the status quo. This is like providing a known drug treatment, or an old version of a website. This is known as the control group. The other group includes the manipulation we wish to test, such as a new drug or new website layout. This is known as our experimental group. We can compare the outcomes between groups (e.g. recovery time or click-through rate) in order to make a judgement about the effect of our manipulation. (Since we have an experiment, we'll randomly assign each unit to either the control or experimental group.) For web-based experiments, this kind of basic experiment design is called an A/B test: the "A" group representing the old control, and "B" representing the new experimental change.

We aren't limited to just two groups. We could have multiple experimental groups to compare, rather than just one control group and one experimental group. This could form an A/B/C test for a web-based experiment, with control group "A" and experimental groups "B" and "C".

If an individual completes all conditions, rather than just one, this is known as a within-subjects design. Within-subjects designs are also known as repeated measures designs. By measuring an individual's output in all conditions, we know that the distribution of features in the groups will be equivalent. We can account for individuals' aptitudes or inclinations in our analysis. For example, if an individual rates three different color palettes for a product, we can know if a high rating for one palette is particularly good compared to the others (e.g. 10 vs. 5, 6) or if it's not a major distinction (e.g. 10 vs. 8, 9).

Randomization still has a part in the within-subjects design in the order in which individuals complete conditions. This is important to reduce potential bias effects, as will be discussed later in the lesson. One other downside of the within-subjects design is that it's not always possible to pull off a within-subjects design. For example, when a user visits a website and completes their session, we usually can't guarantee when they'll come back. The purpose of their following visit also might not be comparable to their first. It can take a lot more effort in control in order to set up an effective within-subjects design.


## Types of Sampling

While web and other online experiments have an easy time collecting data, collecting data from traditional methods involving real populations is a much more difficult proposition. If you need to perform a survey of a population, it could be unreasonable in both time and money costs to try and collect thoughts from every single person in the population. This is where sampling comes in. The goal of sampling is to only take a subset of the population, using the responses from that subset to make an inference about the whole population. Here, we'll cover two basic probabilistic techniques that are commonly used.

The simplest of these approaches is simple random sampling. In a simple random sample, each individual in the population has an equal chance of being selected. We just randomly make draws from the population until we have the sample size desired; your sample size depends on the level of uncertainty you are willing to have about the collected data. Since everyone has an equal chance of being drawn, we can expect the feature distribution of selected units to be similar to the distribution of the population as a whole. In addition, a simple random sample is easy to set up.

However, it is possible that certain groups are underrepresented in a simple random sample, especially those that make up a low proportion of the population. If there are certain rarer subgroups of interest, it can be worth adding one additional step and performing stratified random sampling. In a stratified random sample, we need to first divide the entire population into disjoint groups, or strata. That is, each individual must be a part of one group, and only one group. For example, you could divide people by gender (male, female, other), or age (e.g. 18-25, 26-35, etc.).

Then, from each group, you take a simple random sample. In a proportional sample, the sample size is proportional to how large the group is in the full population. For example, if you require 1000 data points, and stratified individuals of proportion {0.5, 0.3, 0.2}, then you would take 500 people from the first group, 300 from the second, and 200 from the third. This guarantees a certain level of knowledge from each subset, and theoretically a more representative overall inference on the population.

An alternative approach is to take a nonproportional sample from each group. For example, we could simply sample 500 people from each group. Computing the overall statistics in this case requires weighting each group separately, but this extra effort offers a higher understanding of each subgroup in a deeper investigation.
