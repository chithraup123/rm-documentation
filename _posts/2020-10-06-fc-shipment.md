---
layout: post
title: FC Shipment
modified: 10/06/2020, 9:00:24
tags: [intro, beginner, jekyll, tutorial]
comments: true
category: blog
---

**Carrier Info**

Checked if we have values for both 'Tot Billed' from invoice and 'Shipping Carrier' from Carrier Details

**Source Warehouse column to WS list screen**

Shows the Preparation center of the IS

Note: Allows only one to one association between the Warehouse and the preparation center
 

#### FC Shipment Add/Edit

**Paid Ribbon**

Invoice Details : Give Payment Date--> Save it-->Paid Ribbon

**Shipping Cost**

Invoice Details--->'Amount' value should be distributed among all the SKU rows given in the FC based on SKU's CBM

SKU1's CBM = MasterCartonLength(meter) * MasterCartonHeight(meter) * MasterCartonWidth(meter)

SKU1's Total Carton CBM = SKU1's CBM * Total No of Cartons

SKU1's Total Carton CBM % = SKU1's Total Carton CBM / (SKU1's Total Carton CBM + SKU2's Total Carton CBM) * 100

Shipping Cost for SKU1 = Sum of (Amount) from all invoices * SKU1's Total Carton CBM %

**Per Each Shipping Cost**

Shipping Cost/Number of Cartons


