---
layout: post
title: Import Shipments
modified: 10/06/2020, 9:00:24
tags: [intro, beginner, jekyll, tutorial]
comments: true
category: blog
---

##### Calculating Tariff in Inventory Shipment page
The Tariff can be calculated if Manufacture price and Tariff Code is available in UI as following
```sh
Tariff Per Unit = Manufacture Price * Tariff rate %
Total Tariff = Tariff Per Unit * Total Unit Quantity
```
##### Mass Adjust Tariff 

The Tariff can be calculated while uploading Mass Adjust file as following

- Download Template - 
Using this template, user can give the inputs for calculating tariff for the given SKU’s of the inventory. The SKU/Model number can be given as an Identifier

- Upload Adjustment File - 
The SKU with the above given values will get filled in the UI only if this SKU is already present in the UI

##### View Total Tariff By HTS Code
This view contains 6 columns such as HTS code, Tariff %, Total Reported Value, Tariff Costs, MPF(Merchandise Processing Fee), HMF(Harbor Maintenance Fee) and Total Tariff Costs

```sh
Tariff % is based on the Tariff code ie The latest Tariff code modified before the Inventory-->ETA

Tariff Costs = Sum of Tariff Costs for a HTS code(Tariff Cost for single SKU row = Total Reported Value * Tariff %)

MPF = .3464 % of Total Reported Value

HMF = .125 % of Total Reported Value

Total Reported Value will be available only from Mass adjust file
If the file is provided only Reported Unit Value then Reported Total Value = Reported Unit Value  * Total Unit Quantity

Total Tariff Costs = Tariff Costs + MPF + HMF
```
