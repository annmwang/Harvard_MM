---
layout: post
title: MMFE8 conditions
excerpt: "Working conditions of the MMFE8 boards"
categories: [documentation]
comments: true
---

ON = original notes at the beginning of this log

Status of boards, 2017/07/14

| Serial | IP | MAC | Rev | Notes |
|--------|--------|--------|--------|--------|
| 62  | 105 | x05 | C | In the octuplet |
| 159 | 117 | x11 | D | Broken |
| 148 | 107 | x07 | D | In the octuplet |
| 149 | 106 | x06 | D | In the octuplet (no change) |
| 160 | 119 | x13 | D | In the octuplet |
| 114 | 102 | x02 | D | In the octuplet |
| 156 | 116 | x10 | D | In the octuplet (no change) |
| 135 | 118 | x12 | D | In the octuplet |
| 132 | 101 | x01 | D | In the octuplet |
|=====

List of repairs being done by Sarah, 2017/06/01

| Serial | IP | MAC | Rev | VMMs being replaced |
|--------|--------|--------|--------|--------|
| 62  | 105 | x05 | C | 0, 1 |
| 159 | 117 | x11 | D | 1, 7 |
| 148 | 107 | x07 | D | 0, 4, 5 |
| 149 | 106 | x06 | D | N/A |
| 160 | 119 | x13 | D | 0, 1, 2 |
| 114 | 102 | x02 | D | 4, 7 |
| 156 | 116 | x10 | D | |
| 135 | 118 | x12 | D | 3 |
|=====

Log at the end of Run 3523, 2017/05/31

| Serial | IP | MAC | Rev | Notes |
|--------|--------|--------|--------|--------|
| 62  | 105 | x05 | C | VMM 0, 1 are 1/3 dead |
| 159 | 117 | x11 | D | VMM 1, 7 are 1/3 dead |
| 148 | 107 | x07 | D | VMM 0, 4, 5 are all dead/missing a lot of channels |
| 149 | 106 | x06 | D | |
| 160 | 119 | x13 | D | VMM 0, 1, 2 are also all dead |
| 114 | 102 | x02 | D | VMM 4 doesn't have ART signal, VMM 7 is half dead|
| 156 | 116 | x10 | D | |
| 135 | 118 | x12 | D | VMM 3 is funny and shows up in ART but not in MM data, shows up in calibration data |
|=====

Log for 2017/05/11

| Serial | IP | MAC | Rev | Notes |
|--------|--------|--------|--------|--------|
| 62  | 105 | x05 | C | |
| 159 | 117 | x11 | D | |
| 148 | 107 | x07 | D | ON: VMM0 in short |
| 149 | 106 | x06 | D | |
| 160 | 119 | x13 | D | 2017/05/11: VMM2 appears to only have 3 channels left; ON: VMM1 in short, VMM2 has 90% channels dead|
| 114 | 102 | x02 | D | |
| 156 | 116 | x10 | D | |
| 135 | 118 | x12 | D | 2017/05/11: VMM3 shows up in calibration runs, but *not* in the cosmic data since board installation|
| 130 | 109 | x09 | D | |
| 132 | 101 | x01 | D | |
| 639 | 111 | x0b | C | |
| 642 | 112 | x0c | C | |
| 641 | 120 | x14 | C | 2017/05/10 flash replaced |
| 643 | 121 | x15 | C | |
| 163 | 113 | x0d | D | |
| 164 | 114 | x0e | D | |
| 151 | 115 | x0f | D | |
|=====

