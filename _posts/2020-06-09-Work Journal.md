---
layout: post
title: Work Journal of 06/09
date: 2020-06-09
summary: Breif journal of today work
categories:
visibility: public
---
# Work Journal of 06/09/2020

## What I've done today
1. Esabblished the backend support of handling report type favorite
2. Esablished the worskflow of creating dynamic searching query param on front end and backend

## What problem I've found
1. Razor did not parse c# code to html on partial view

## Why it happen?
1. User `jQuery.load(url, parameter)` as well as PartialViewResult controller method to generate the partial view
2. (Potential) No `<html>` tag as the outter element of partial view html page as it will lead to seperate DOM 
3. Normally if the partial view is not generated dynamically, use `@Html.RenderPartial()` instead of `jQuery.load()`

## How long did I spend on the problem
Nearly 3~4 hours

## How to reduce the working time on such similar problem
1. Suggest learn logic of how Razor parses the `.cshtml` file and pass it into the page as well as update DOM on browser