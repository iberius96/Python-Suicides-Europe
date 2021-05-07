## Project rationale & objective

The data analysis project contained in this notebook aims to study the behavior of suicide rates in European countries in relation to a set of chosen labour market features.

The rationale for this work is the assumption that the changing trends in the labour market (and consequently in the economical and social structure of a given country) are strong driving factors in influencing the suicide rate values.

By visualizing and correlating suicide rate data with labour market features, we will try to verify the existence of this relationship, together with a measure of its strength.

Additionally, we will try to utilize machine learning techniques to create one or more models that, given a set of labour market features, will allow us to obtain an estimate of the expected suicide rates.

## Summary

After a brief initial description to contextualize this work, together with some preliminary operation needed to set up our notebook, we spent the first portion of this project conducting a fairly in-depth curation process which was required to obtain usable datasets for both suicide and labour market data.

An interesting but also challenging aspect of preparing our data was certainly the choice of using two different sources to obtain a more complete overview of the suicide rates in Europe. This introduced the challenge of performing some additional preparation steps to make sure that our two datasets could be joined together.

Another interesting section of this work was the contextualization of outliers. It is noticeable how, at the end of this process, we decided to keep all the countries containing the bulk of our outliers. The reasoning behind this decision was that the factors causing high suicide rate values (like the fall of the Soviet Union) would also influence the labour market data values.

A similar (although briefer) curation process was also conducted for the labour market data.

After these initial preparation steps, we decided to perform a set of visualizations required to obtain a deeper insight in relation to the datasets we were working with. This portion of our work was more focused on the complete representation of the suicide dataset.

After joining the labour market and suicide datasets together and providing an overview in regards to the correlation of the various features, we then decided to conclude our project by creating a set of machine learning models trained on our complete data.

An interesting aspect related to this part of our work was finding a good balance between the number of selected labour market features and the pool of data rows that we could use for machine learning.

Using a very small number of labour market features would have not provided enough information to obtain acceptable model scores. At the same time, adding too many features would have reduced the total nr of usable (i.e. not containing Na values) rows that we could provide to our models.

Settling for six labour market features + an additional one (sex) provided us with enough granularity to build models that were able to predict suicide rate values in a pretty accurate manner.