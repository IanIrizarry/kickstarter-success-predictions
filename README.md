# Predicting Kickstarter Success

## Problem Statement
-----

As somone interested in creating my entrepreneurs in the world, I thought it would be a good idea to see if I could take several years of Kickstarter data and see if I can predict whether a project would be successful or not and then use that information to make recommendations for those interested in creating something for themselves. But first, I needed to answer the following:

>  Can a model be created that predicts the success of a project on Kickstarter, greater than the baseline rate?


## Executive Summary
----
Kickstarter is a crowdfunding platform that helps inspired creators receive the funding they need to bring their ideas to life. What makes the platform unique is that it is that it attracts people in all financial classes to the platform to invest in ideas. This provides a unique opportunity for future creators because he shows real market interest in products and ideas that have yet to be created. Future creators can use this knowledge to inspire their own ideas by using Kickstarter data to find ideas that they support and create products based on those ideas. However, the purpose of this research is to take creators past simply picking topics by interest and, instead, helping them pick by more objective features.

In this research, my goal was to see whether or not I could predict success given the data of a product on Kickstarter. Using that data, I created a logistic regression model to predict whether or not a project would be successful. The baseline, or percentage of successes of total observations was 65%. Seperating out over 200 features and running 4 models, three models covering a category and the fourth covering all categories, I was able to determine that there were features that greatly influenced success: the number of backers and the financial goal. After filtering out as many variables I could, my predictions after tuning the model was roughly 85% for all four models.

For creator's using this model, they will find that for every backer that they gain, their liklihood of success increases dramatically. However, they will also find that the larger their financial goal, the lower their chances of succeeding are as well.

----

## Conclusion
------
To conclude, everyone has the capacity to create something unique. What may be lacking is inspiration. We can use Kickstarter for that. There are a lot of successful projects on Kickstarter and we know that people are willing to bet their money on an idea. So, we use those ideas that we like and build on them. Then, with the right goals and the people to support us, we can achieve what we want to achieve.

### Recommendation
First, since category and sub-category didn’t really influence whether a project was successful or not, creators should choose topics that interests them. If they don’t love the topic, it will be much harder for them to create in that space.

Once you have the category is decided on, then they can focus on backers. If they choose the category food and the subcategory accessory (for example), they can see what the average number of backers is and make that their goal to achieve.

Finally, once they have a good idea of how many backers they should aim for, they also need to consider their financial goal. I’d recommend doing the same thing as my recommendation for the number of backers: try to keep the financial goal within the ball park of other successful projects in that category. However, there is a balance that needs to be considered: if the project requires ‘x’ number of dollars, and the goal number of backers is ‘y’, the larger the goal, the more impact it will have on your investment per backer. So just keep that in mind.


## Data Dictionary

At the time of this writing, no data dictionary can be found so I have to make some assumptions as to what some of these features are based on research on the terms. For terms that I cannot explain, they will likely be removed unless they provide substantial meaning. At this point (July 15, 2020), I have decided to leave the variables listed here for reference but leave the dashes for variables I could not find explanations for.

After all of the missing values were removed, 34 columns remained:

||Feature|Data Type|Description|
|--------|--------|--------|-------|
|1|Backers count|integer|number of backers supporting the project|
|2|Blurb| text|text that describes the project|
|3|Category|object|a string of text that includes the project ID, the 'name' of the project, 'slug' which includes the name and the broader category that the project falls into, position number, parent id, parent name (the broader category), color number, and the url|
|4|Converted pledged amount|integer| -------------- |
|5|Country|nominal| Country name abbreviated
|6|Country displayable name|nominal|Full country name displayed|
|7|Created at|timestamp| ----------------|
|8|Creator|object|--------------------|
|9|Currency|nominal| ----------------|
|10|Currency symbol|nominal| the symbol for the type of currency|
|11|Currency trailing code|boolean| ----------|
|13|Deadline|integer|--------|
|14|Disable communication|boolean|----------------------|
|15|FX_rate|float|-----------|
|16|Goal|float|Financial goal needed to achieve a successful project|
|17|ID|integer| ID of the project|
|18|Is starrable|integer| ---------------- |
|19|Launched at|integer| ------------------|
|20|Location|string| ---------------------- |
|21|Name|text| description of category|
|22|Photo|object| --------------------|
|23|Pledged|float| Dollars pledged|
|24|Profile|object| ----------------- |
|25|Slug|object| -------------------- |
|26|Source url|object| url of the project|
|27|Spotlight|bool| did project appear in Kickstarter's spotlight program (perfectly predicts success|
|28|Staff pick|bool| -------------- |
|29|State|nominal| example: success or failure|
|30|State changed at|int| ----------------|
|31|Static usd rate|float|------------------|
|32|Urls|object| ------------------|
|33|USD pledged|float| pledged amount in USD|
|34|USD type|object| domestic or international|