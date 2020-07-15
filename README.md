# kickstarter-success-predictions

At the time of this writing, no data dictionary can be found so I have to make some assumptions as to what some of these features are based on research on the terms. For terms that I cannot explain, they will likely be removed unless they provide substantial meaning.

After all of the missing values were removed, 34 columns remained:

||Feature|Data Type|Description|
|--------|--------|--------|-------|
|1|Backers count|integer|number of backers supporting the project|
|2|Blurb| text|text that describes the project|
|3|Category|object|a string of text that includes the project ID, the 'name' of the project, 'slug' which includes the name and the broader category that the project falls into, position number, parent id, parent name (the broader category), color number, and the url|
|4|Converted pledged amount|integer| -------------- |
|5|Country|nominal| --------------|
|6|Country displayable name|nominal|----------------|
|7|Created at|timestamp| ----------------|
|8|Creator|object|a string of text that includes the project ID, the 'name' of the project, 'slug' which includes the name and the broader category that the project falls into, position number, parent id, parent name (the broader category), color number, and the url|
|9|Currency|nominal| ----------------|
|10|Currency symbol|nominal| the symbol for the type of currency|
|11|Currency trailing code|boolean| ----------|
|13|Deadline|integer|--------|
|14|Disable communication|boolean|----------------------|
|15|FX_rate|float|-----------|
|16|Goal|float|--------------|
|17|ID|integer| number of backers supporting the project|
|18|Is starrable|integer| number of backers supporting the project|
|19|Launched at|integer| number of backers supporting the project|
|20|Location|integer| number of backers supporting the project|
|21|Name|text| --------------------|
|22|Photo|integer| number of backers supporting the project|
|23|Pledged|integer| number of backers supporting the project|
|24|Profile|integer| number of backers supporting the project|
|25|Slug|integer| number of backers supporting the project|
|26|Source url|integer| number of backers supporting the project|
|27|Spotlight|integer| number of backers supporting the project|
|28|Staff pick|integer| number of backers supporting the project|
|29|State|nominal| number of backers supporting the project|
|30|State changed at|integer| number of backers supporting the project|
|31|Static usd rate|integer| number of backers supporting the project|
|32|Urls|integer| number of backers supporting the project|
|33|USD pledged|integer| number of backers supporting the project|
|34|USD type|integer| number of backers supporting the project|