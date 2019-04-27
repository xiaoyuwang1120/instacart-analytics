---
layout: page
title: Feature Engineering
bigimg: /img/reorder.jpg
---

Based on user aspect with **user_id** as primary key, construct data_all1

1．	Reorder times
```
gmcs=orders_prior.groupby(['user_id'])['order_id'].count()
gmcs=pd.DataFrame(gmcs)
gmcs['user_id']=gmcs.index
gmcs.columns=['gmcs','user_id']
```
2．	Reorder time interval
```
gmpl=orders_prior.groupby(['user_id'])['days_since_prior_order'].mean()
gmpl=pd.DataFrame(gmpl)
gmpl['user_id']=gmpl.index
gmpl.columns=['gmpl','user_id']
```
3．	Reorder ratio
```
user_fgl=data2.groupby('user_id')['reordered'].mean()
user_fgl=pd.DataFrame(user_fgl)
user_fgl['user_id']=user_fgl.index
user_fgl.columns=['user_fgl','user_id']
```
4．	The number of products in each order on average
```
product_num_everytime=product_num_everytime.groupby('user_id')['product_num_everytime'].mean()
product_num_everytime=pd.DataFrame(product_num_everytime)
product_num_everytime['user_id']=product_num_everytime.index
product_num_everytime.columns=['product_num_everytime','user_id']
```
5．	The number of products in total
```
num_product=data2.groupby('user_id')['product_id'].count()
num_product=pd.DataFrame(num_product)
num_product['user_id']=num_product.index
num_product.columns=['num_product','user_id']
```
6．	The number of distinct products
```
num_distinct_prodct=data2.groupby('user_id')['product_id'].apply(f1)
num_distinct_prodct=pd.DataFrame(num_distinct_prodct)
num_distinct_prodct['user_id']=num_distinct_prodct.index
num_distinct_prodct.columns=['num_distinct_prodct','user_id']
```
7． reorder ratio of the last order
```
data2_last_order=data2.groupby('user_id')['order_number'].max()
data2_last_order=pd.DataFrame(data2_last_order)
data2_last_order['user_id']=data2_last_order.index
data2_last_order.columns=['num','user_id']
data2_last_order=pd.merge(data2,data2_last_order,on='user_id',how='left')
data2_last_order=data2_last_order[data2_last_order.order_number==data2_last_order.num]
data2_last_order=data2_last_order.groupby('user_id')['reordered'].mean()
data2_last_order=pd.DataFrame(data2_last_order)
data2_last_order['user_id']=data2_last_order.index
data2_last_order.columns=['last_order_reorderd','user_id']
```
Based on products aspect with **product_id** as primary key, construct data_all2
1.	the number of orders and its ratio in total orders
```
product_of_order_num=data2.groupby('product_id')['order_id'].count()
product_of_order_num=pd.DataFrame(product_of_order_num)
product_of_order_num['product_of_order_num']=product_of_order_num.index
product_of_order_num.columns=['product_of_order_num','product_id']
```
2.	the number of ordered users
```
product_of_user_num=data2.groupby('product_id')['user_id'].apply(f1)
product_of_user_num=pd.DataFrame(product_of_user_num)
product_of_user_num['product_of_user_num']=product_of_user_num.index
product_of_user_num.columns=['product_of_user_num','product_id']
```
3.	the number of reorders
```
product_of_second_order_num=data2[data2.reordered==1].groupby('product_id')['order_id'].count()
product_of_second_order_num=pd.DataFrame(product_of_second_order_num)
product_of_second_order_num['product_of_second_order_num']=product_of_second_order_num.index
product_of_second_order_num.columns=['product_of_second_order_num','product_id']
```
4.	the number of reordered users
```
product_of_second_user_num=data2[data2.reordered==1].groupby('product_id')['user_id'].apply(f1)
product_of_second_user_num=pd.DataFrame(product_of_second_user_num)
product_of_second_user_num['product_of_second_user_num']=product_of_second_user_num.index
product_of_second_user_num.columns=['product_of_second_user_num','product_id']
```
5.	product reorder ratio
```
product_fgl=data2.groupby('product_id')['reordered'].mean()
product_fgl=pd.DataFrame(product_fgl)
product_fgl['product_id']=product_fgl.index
product_fgl.columns=['product_fgl','product_id']
```
6.	add to cart order
```
product_location=data2.groupby('product_id')['add_to_cart_order'].mean()
product_location=pd.DataFrame(product_location)
product_location['product_id']=product_location.index
product_location.columns=['product_location','product_id']
```


