---
name: How is Hardship Defined Across Chicago Neighborhoods?
tools: [Python, Altair, vega-lite]
description: Visualizing socioeconomic indicators across Chicago neighborhoods
---

# How is Hardship Defined Across Chicago Neighborhoods?

*Author: Luke Hull*

The City of Chicago tracks different socioeconomic indicators across its 77 neighborhoods or community areas, calculating a composite score called Hardship index. It considers income, unemployment, housing crowding, poverty, education, and age. These statistics, tracked from 2008 to 2012 help the city understand how hardship is distributed across its neighborhoods. They influence policymakers, researchers, and residents and allow them to identify where resources and interventions are most necessary. These visualizations explore the distribution of these indicators in conjunction with each other across city using data from the publicly-available Chicago Data Portal (cited below).

Chicago has a rich but troubled history. Redlining practices, their lingering effects, and institutional racism have plagued many urban areas with Chicago being no exception. This segregation still shows its effects in many ways including wealth gaps, education disparity, and economic disadvantage. While visualizing socioeconomic indicators in Chicago, it would be irresponsible to ignore the history that contributes to disparities across its neighborhoods.

## Contextual Visualization 1: Racial Borders in Chicago (2010)

<img src = '{{ site.baseurl }}/assets/pngs/segregation-2010-map-01_01.png'>

*Source: WTTW - Mapping Chicago's Racial Segregation (https://www.wttw.com/firsthand/segregation/mapping-chicago-racial-segregation)*

This dop map illustrates the racial segregation across Chicago's neighborhoods as recently as 2010. These dots, colored by race, show strong petterns with White residents concentrated on the North Side, Black residents concentrated in the South and West Sides, and Latino residents in areas between. While these visualizations do not examine the grographic distribution of these socioeconomic indicators and hardship scores, it is important to recognize the segregation across Chicago and note the potential influence.

## Contextual Visualization 2: Wealth Disparities by Race and Ethnicity through Time (1963-2022)

<img src = '{{ site.baseurl }}/assets/pngs/average-family-wealth-by-race-and-ethnicity-1963-2022.png'>

The second contextual chart from the Urban Institute shows average family wealth by race and ethnicity from 1963 to 2022. While White families have seen their wealth grow dramatically over the past six decades, Black and Hispanic families have remained largely unchanged, comparatively, in the same period. This growing wealth gap nationally provides critical context for the income disparities seen across Chicago neighborhoods, especially considering the racial segregation still present in the City.

## Exploring the Data

Through this interactive scatterplot, choose one of the six socioeconomic indicators to see how it is distributed compared to, and correlates with Hardship Index across all neighborhoods with a trendline to accentuate the relationship. Hover over any of the points to see the name of the neighborhood along with its calculated Hardship Index.

<vegachart schema-url="{{ site.baseurl }}/assets/json/mainScatter.json" style="width: 100%"></vegachart>

Examining trends across the different socioeconomic indicators helps to illustrate how they relate to and potentially impact the calculated hardship score that an aggregation of them. We can see the most clear correlations between hardship, households below poverty, and per capita income. There is a strong positive association between housholds below poverty and hardship, while a strong negative between hardship and per capita income (while it does not appear to be a linear association). Past this, we can also see a positive association, albeit weaker, between hardship and unemployment, housing crowding, education, and age. While further analysis is needed to determine any kind of causal relationship or influence on the hardship value, their associations give some insight into how hardship is measured in Chicago.

## Conclusion

Overall, there are many factors that contribute to these socioeconomic indicators across Chicago neighborhoods. Through examining these associations and other contextual considerations, it is clear that hardship in Chicago is not the result of individual circumstances but rooted in structural and historical forces that continue to affect communities today. Understanding these patterns is the first step towards policy decisions and interventions to bridge socioeconomic disparities across Chicago and other urban areas.

<div class="left">
{% include elements/button.html link="https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2/about_data" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/lhull3/lhull3.github.io/tree/main/python_notebooks/finalproject.ipynb" text="The Analysis" %}
</div>

