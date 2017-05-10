---
layout: post
title: TP Data Info
excerpt: "Useful information about the TP data"
categories: [documentation]
comments: true
---

#### Board ordering in fitter packet data
[V1  V0]

[U1  U0]

[X3  X2]

[X1  X0]

Alternatively, where the boards are indexed in increasing z:

[5, 3, 4, 2, 7, 6, 1, 0]

#### TP + GBT BCID matching
Currently, the BCID reported in the TP is taken from the **second** packet in the GBT buffer (where we have alternating packets from the two ADDCs).

This currently corresponds to packets from **ADDC B**, which feeds in data from MMFE8 boards 0-3.

#### ADDC and TP configuration

ADDC A: [A1 A2 A3 A4]

ADDC B: [B1 B2 B3 B4]

