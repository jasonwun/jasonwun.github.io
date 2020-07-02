---
layout: post
title: Work Journal of 07/01
date: 2020-07-01
summary: Breif journal of today work
categories:
visibility: public
---

## Plan of today
### Implementation Category
#### Complete MKT-859 database refactoring

1. Redesign table
2. Create Migration logic
    * Copy records from MKT_ISO_NITS_Rate to MKT_LDC_Published_Charge
    * Add new column in PRC_Iso_State_Charge_Item named Charge_Column_Name and map the `NITSCh` data name
3. Update Nits Rate page
    * Update Get Iso Nits Rate Stored proc
    * Update Save Iso Nits Rate Stored proc
    * Update Approve Iso Nits Rate Stored proc
    * Update Reject Iso Nits Rate Stored proc
    * Create new Column name constant for the new column
    * Adapt the Nits Rate page for newly updated stored proc
#### Compelte Michael's USG-2287
#### Adjust Control Entity of Report Console
1. Redesign table
2. Create Migration logic
    * Copy records from MKT_ISO_NITS_Rate to MKT_LDC_Published_Charge
    * Add new column in PRC_Iso_State_Charge_Item named Charge_Column_Name and map the `NITSCh` data name
3. Update Nits Rate page
    * Update Save Iso Nits Rate Stored proc
    * Update Get Iso Nits Rate Stored proc
    * Update Reject Iso Nits Rate Stored proc
    * Create new Column name constant for the new column
***

## What I've really done today
### Implementation Category
#### Complete MKT-859 database refactoring
1. Redesign table
2. Create Migration logic
    * Copy records from MKT_ISO_NITS_Rate to MKT_LDC_Published_Charge
    * Add new column in PRC_Iso_State_Charge_Item named Charge_Column_Name and map the `NITSCh` data name
3. Update Nits Rate page
    * Update Get Iso Nits Rate Stored proc
    * Update Save Iso Nits Rate Stored proc
    * Update Reject Iso Nits Rate Stored proc
#### Compelte Michael's USG-2287
*** 

## What Left?
1. The biggest issue of the Approve Nits Rate Stored proc is how to approve the record that has the same value of its archived data, which means adding the archived status. If we update the records' status directly by [Status] then it will hit unique index problem.

2. The second problem is that the reopened Report Console problem. I believe I should make it done by tomorrow once

## The problem
So far there are so many tickets stuck in my backlog. After I've cleared the current one. I should finish those which has the longest working time