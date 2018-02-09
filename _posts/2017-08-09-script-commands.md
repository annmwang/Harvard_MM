---
layout: post
title: Script commands
excerpt: "Script commands for fast reference"
categories: [code]
comments: true
---

## Merging scintillator, MM, and optionally tp files

{% highlight shell %}
python merge_time.py -m mm.dat -s ss.dat -t [t.dat] --offset -o output.dat
{% endhighlight %}

## TP decoding:

{% highlight shell %}
python decodeGBT_32bit.py --ifile IFILE --ofile OFILE
python decodeTIME_32bit.py --ifile IFILE --ofile OFILE
python decodeFIT_uvr.py -i <inputfile> -o <outputfile> -r <run> -f [--sl] [--st]
{% endhighlight %}
Various flags for the FIT decoder: ```-f``` to add strip offsets (put this in!!!!), ```-r``` (the strip offsets are dependent on the run #), ```--sl``` to decode the slopes OR ```--st``` to decode the strips

Deprecated:
{% highlight shell %}
python decodeFIT_32bit.py -i <inputfile> -o <outputfile> -r <run> -f [-s]
{% endhighlight %}

Various flags for the FIT decoder: ```-f``` to add strip offsets (put this in!!!!), ```-s``` optionally to decode strips and slopes as opposed to just strips

