---
layout: post
title: Starting a run, for P.G.
excerpt: "Starting a run for fast reference"
categories: [documentation]
comments: true
---
Order of operations:

#### Turn on HV

#### Delete old DAQ files 
* Go to /data/mm_2016/work/
* Delete anything called mmtp_*.dat
* Delete mmfe8TestQuiet.dat

#### Power cycle + Configure boards
* Wait until you can talk to the MMFE8s
* Go to /data/mm_2016/mm_daq/python/

{% highlight shell %}
python jonah_config.py 8 <location of config file>
{% endhighlight %}

* Configuration files are located in /data/mm_2016/mm_daq/config/
* Should be labeled by run, or use the latest one.

* Wait until configured

#### Start scintillator DAQ / open crate

#### Start MM DAQ
{% highlight shell %}
python data_acq_multi_mmfe8_seq.py 8
{% endhighlight %}

* Type in IPs of board when prompted
* Type in 1 to start DAQ

#### Start Trigger DAQ

* If the output FIFOs have not been enabled, you need to enable them. Generally this only needs to be done once after the TP is programmed.
* To enable the output FIFOs:
* Go to /data/mm_2016/trigger_daq

{% highlight shell %}
python regWrite.py --df "1110"
{% endhighlight %}

* This enables FIFOs 21, 22, 23. 
* Once the output FIFOs have been enabled, to turn on the DAQ:

{% highlight shell %}
python udpRecDesp_32bit.py
{% endhighlight %}

#### Change the priority of both the MM DAQ and the TP DAQ

{% highlight shell %}
sudo renice -18 -p <PID>
{% endhighlight %}


