---
layout: page
title: Feature Engineering
bigimg: /img/reorder.jpg
---

Based on user aspect with user_id as primary key, construct data_all1

1．	Reorder times

```
gmcs=orders_prior.groupby(['user_id'])['order_id'].count()
gmcs=pd.DataFrame(gmcs)
gmcs['user_id']=gmcs.index
gmcs.columns=['gmcs','user_id']
```
2．	Reorder time interval
3．	Reorder ratio
4．	The number of products each order in average
5．	The number of products in total
6．	The number of distinct products
7．	Last order reorder ratio
8．	Time of last order/reorder ratio
9．	The number of products of last order/the number of average products


## Or some code?

Some code might go here:

```
x <- 5 # Here's some R code
```

What if I just paste the HTML for a plotly plot?

We can do it with a line of markdown that looks like this (without the slashes - I haven't solved that problem just yet...):
```
\{\% include jupyter-basic_bar.html \%\}
```
{% include jupyter-basic_bar.html %}
