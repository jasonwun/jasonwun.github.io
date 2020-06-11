---
layout: post
title: Work Journal of 06/10
date: 2020-06-10
summary: Breif journal of today work
categories:
visibility: public
---
# Work Journal of 06/10/2020

## What I've done today
1. Established the dynamic mechanism of generating kendo grid columns and data.
<p>For the mechanism, the original thought is that we need to create a mechanism so that the corner stone of Report Console can handle different report type's requirents like search query params as well as data grid columns</p>
<p>Currently the table stores the type specific search param and columns data in json string. The reason why I choose json string is because it is flexible enough to support different demand of different report type. For particular report type, we only need to update or insert the latest json string format so that we don't have to use database table to cover different scenario. </p>
<p>However, there is drawback that, for search param, developer has to take responsibility to validate the json string. Validation for columns and datas won't be a problem because the data is searlized and inserted into database by Report Generator. </p>

2. Attend the traning session and learn basic knowledge of Messageing and Settlement module
#### Messaging 
<p>The purpose of messaging module is that most of the features in ArcTrade are turned into event driven and messaing module would help the achieve that. </p>
<p>Based on Michael descripton, the Messaing module is basically a message queue and each module would describe the queue for receiving the latest message</p>
<p>However, Micheal didn't explain why he choose Database based Messaing rather than other typical open sourceMessaing solution. I've read some articles about the database solution but I want to know more about what does Michael think of that. Also, I' still a little bit doubt that the sequential dequeue approach. Maybe I don't know the overal message throughput per da. </p>

#### Settlement
<p>The Settlement module defined as handling both Billing and Quotation issue. Today Fong shown us alot about how the module store and generate the invoce report of PJM. To be honest, I still don't know a lot about the module even though I was during the session.</p>