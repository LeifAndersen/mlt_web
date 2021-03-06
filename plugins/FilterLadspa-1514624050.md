---
layout: standard
title: Documentation
wrap_title: "Filter: ladspa.1514624050"
category: plugin
---
* TOC
{:toc}

## Plugin Information

title: ZamGateX2  
media types:
Audio  
description: LADSPA plugin  
version: 1  
creator: Damien Zammit  
copyright: Copyright (C) 2004-2014 Meltytech, LLC  
license: GPLv2  
URL: [http://www.ladspa.org/](http://www.ladspa.org/)  

## Notes

Automatically adapts to the number of channels and sampling rate of the consumer.

## Bugs

* Some effects have a temporal side-effect that may not work well.


## Parameters

### 4

title: Attack    
type: float  
readonly: no  
required: no  
minimum: 0.1  
maximum: 500  
default: 125.075  

### 5

title: Release    
type: float  
readonly: no  
required: no  
minimum: 0.1  
maximum: 500  
default: 100  

### 6

title: Threshold    
type: float  
readonly: no  
required: no  
minimum: -60  
maximum: 0  
default: -60  

### 7

title: Makeup    
type: float  
readonly: no  
required: no  
minimum: -30  
maximum: 30  
default: 0  

### 8[*]

title: Output Level    
type: float  
readonly: true  
required: no  
minimum: -45  
maximum: 20  
default: -45  

### 9[*]

title: Gain Reduction    
type: float  
readonly: true  
required: no  
minimum: 0  
maximum: 40  
default: 0  

### instances

title: Instances    
description:
<pre>
The number of instances of the plugin that are in use.
MLT will create the number of plugins that are required to support the number of audio channels.
Status parameters (readonly) are provided for each instance and are accessed by specifying the instance number after the identifier (starting at zero).
e.g. 9[0] provides the value of status 9 for the first instance.
</pre>
type: integer  
readonly: true  
required: no  

### wetness

title: Wet/Dry    
type: float  
readonly: no  
required: no  
minimum: 0  
maximum: 1  
default: 1  

