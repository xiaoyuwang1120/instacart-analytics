---
layout: page
title: Train & Test
subtitle:
bigimg: /img/grocery.jpg
---

Based on users & products, construted features
1.	How many orders do users order these products?
2.	How many orders do users not reorder these products?
3.	What are the first orders and last orders of users?
4.	How many days do users not reorder these products?
5.	What are the reorder ratios of these products?

Before constructing these features, we need to specify **positive and negative** examples for more reasonable classification. Also, we need to include negative examples in training set. 

**Positive and Negative examples?

a.	Creating data2, merge all six files 
b.	Creating data3, deleted all users' last orders from data2
c.	Creating data4, selected all users' last orders from data2 

Positive Samples: data4
Negative Samples: data_label10

Considering non-reordered products in all users' last orders. 
Since the reorder ratio of last order is 0.6, we selected 70% products from previous orders of each user, and 30% from all products. Merged together as negative examples.
```
user_id=[]
product_id=[]
data_label0=pd.DataFrame()
for i in user_id_all:
    product_id=random.sample(map_dict[i],int(len(map_dict[i])*0.7*0.3))
    product_id.extend(random.sample(product_id_all,int(len(map_dict[i])*0.3*0.3)))
    user_id=[i]*len(product_id)
    a=pd.DataFrame(user_id)
    a['product_id']=product_id
    data_label0=data_label0.append(a)
data_label0.columns=['user_id','product_id']
```
