---
layout: post
title: Work Journal of 07/02
date: 2020-07-02
summary: Breif journal of today work
categories:
visibility: public
---

## Plan of today
### Think Category
#### Confirm the logic of versioning on MKT_LDC_Published_Charge table

### Implement Category
#### Complete Nits Rate Stored procedure
#### Fix USG-2291
#### Fix USG-2287
***

## What I've really done today
### Think Category
#### Confirm the logic of versioning on MKT_LDC_Published_Charge table
Basically the logic is that we only take care of the effective date and effective end date and the actual value. If the newly record has the same effective date and end date and value then discard the newly record; or we have same effective date but different value we delete the old one and update the newly one to production so that we don't have any hisoty record of same value
### Implement Category
#### Fix USG-2291
#### Fix USG-2287
*** 

## What Left?
1. The stored procedure of Nits Rate needed to be changed again as we confirm the the final logic of the table versioning