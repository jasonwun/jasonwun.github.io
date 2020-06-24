---
layout: post
title: Work Journal of 06/23
date: 2020-06-23
summary: Breif journal of today work
categories:
visibility: public
---

<p>So today spent almost like couple of hours to settle down the table design. Michael was so busy to answer my question and thanksfully I was still able to find YuZhi to fix the issue.</p>


---
## Plan of today

### Think Category
#### Settle Down the Database table design of Capacity Auction Result

### Implement Category
#### Implement Excel file parsing logic

***

## What I've really done today
### Think Category
#### Settle down the Database table design of Capacity Auction Result
Discussed with YuZhi and we settled down a design that split the entre Capacity Auction Result into 3 tables which the first one contains the values of common value like `Published Date`, `Effective Start Date` etc. The second table stored the Column Name and its corresponding charge item id. The third one would store actual valud for each column.

### Implement Category
#### Implement the excel parsing logic (In-complete)
This is acutally not completed yet. One of the reaons is that the logic is largly depends on what parameter of Stored procedure accept. So the logic of stored procedure has higher priority than the excel parsing

***

## What problem left?
So the excel parising priority is moved after stored procedure. Once the stored procedure is done and the input parameters are settle down, we are good to continue the excel parsing

Another problem is that, the naming of table and corresponding the controller and stored proc. Capacity Auction Result is for PJM only but the naming is too convention. Should we continue on current naming or we should state the PJM on name