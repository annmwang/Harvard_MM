---
layout: post
title: Script commands
excerpt: "Script commands for fast reference"
categories: [code]
comments: true
---

## Merging scintillator, MM, and optionally tp files

{% highlight shell %}
python merge.py -m mm.dat -s ss.dat -t [t.dat] --offset -o output.dat
{% endhighlight %}

## TP decoding:

{% highlight shell %}
python decodeGBT_32bit.py --ifile IFILE --ofile OFILE
python decodeTIME_32bit.py --ifile IFILE --ofile OFILE
python decodeFIT_32bit.py -i <inputfile> -o <outputfile> -r <run> -f [-s]
{% endhighlight %}

Various flags for the FIT decoder: -f to add strip offsets (put this in!!!!), -s optionally to decode strips and slopes

