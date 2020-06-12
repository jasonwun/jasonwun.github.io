---
layout: post
title: Work Journal of 06/11
date: 2020-06-11
summary: Breif journal of today work
categories:
visibility: public
---
# Work Journal of 06/11/2020

## What I've done today
1. Finally compelte the infrastrcuture of Report Console Module
<p>Right now the Report Console is able to dynamically generate the Search Form as well as the data grid in partial view</p>
<p>The next step is start working on the actual Report Type implementation</p>


## What problem I've met today
1. At the time I need to serialize the form data into plain string, it always return empty string even there are data in the input control. The document of jQuery mentions that the `.serialize()` requires the each form input element is a `Successful Control` which need to fit the following criteria: 
      1. Has its control name paired with its current value as part of the submitted form data set
      2. Must be defined within a FORM element and must have a control name

## What I need to do tomorrow
1. Think about how to design the Generator in OOD fashion. 
2. Discuss with the Generator design with Michael
3. Start working on the implementation of Mass Market Customer List 