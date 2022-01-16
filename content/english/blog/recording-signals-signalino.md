---
id: "0005"
title: "Recording brain signals with Signalino"
date: 2019-07-21T15:45:23+02:00
draft: false
image : "images/blog/1_600.jpg"
bg_image: "images/feature-bg.jpg"
categories: ["Company News"]
tags: ["Advice","Technology"]
description: "this is meta description"

summary: "La Comisión Europea respalda el sistema potenciador de memoria MemBoost"
description: "La Comisión Europea respalda el sistema potenciador de memoria MemBoost"
author:
---

## Introduction

In Signalino we are makers from the very beginning, and we support the
Do It Yourself (DIY) movement, teamwork, obtaining and producing
knowledge in community. We believe in a change of mentality that helps
us to share ideas, projects and develop them together. This is why
 Signalino develops tools that allow all the “makers” to push their
ideas and remove them from the drawers. If you want a good introduction
to fab lab concept, [here you have one (from UA)](http://fablab.ua.es/que-es-fab-lab/).


Biosignals, as EEG, EMG and ECG are, are a great resource for research
in physiology: health or exercise monitoring, neurofeedback or EEG
biofeedback training, experiments with brain-computer interfaces or
simply want to have a look at their brain or heart or muscles at work.

Unfortunately, commercial EEG/ECG devices are usually too expensive to
become a hobbyist tool or toy. Our answer is  signalino:  we have developed  software and hardware for
do-it-yourself bioamplifier devices available for free (as in GPL). 


## Our solution: an Arduino shield

![article-img-centered](/img/blog/0001/EEG2_600.png)

Signalino Shield is a powerful  opensource tool for those who want to
register biosignals and collect data to launch their projects. For this
reason, we encourage Signalino users to share with us their ideas and
projects. We belong to the open community, and we’d love seeing a strong
community growing around some of our products.

{{< youtube O9Kai4d3IyU >}}

[Signalino’s main board](http://www.signalino.com/products) depends
on Arduino. The 32bit OpenBCI Board is a shield for 32-bit Arduino-Due
which converts it in an impressive 8-channel biosignal amplifier.

![article-img](/images/blog/signalino_prototipo_600.jpg)

It is a Hardware development platform for medical devices and eHealth
applications to all those hardware developers, researchers and makers
who need to read biometric signals. It is a mobile kit that measures ECG
and EEG:**[ open-source EEG/ECG Shield for Arduino-Due 32bit Biosignal
Amplifier Board Kit (8-channel)](http://www.signalino.com/tienda/). **

Signalino is aimed toward amateurs who would like to experiment with
biosignals. And, if you are a pro in any of the fields of electronics,
neurofeedback, software development etc, you are of course welcome to
join our community.

All you need is an arduino Due, a  USB cable with a type C connector and
some electrodes, which number depends on the configuration: two for each
bipolar channel or one for each monopolar referenced to some common
electrode  and 1 passive electrode for DRL (the electrodes are sold
separately). Buy one of our kits for 199€, download the software, and
you are recording!

{{< youtube NhLkvW6aybU >}}


#<http://www.signalino.com/wp-content/uploads/2016/12/Signalino-Test1.mp4>

<!---
%<div class="youtube-container">
%            <iframe src="http://www.signalino.com/wp-content/uploads/2016/12/Signalino-Test1.mp4" frameborder="0" allowfullscreen></iframe>
%          </div>
-->
## Technical description

Sure some of the tecnical guys will be interested in details, so let's be more specific: 

### Product Overview:

The 32bit OpenBCI Board is a shield for 32-bit Arduino-Due which converts it in a 8-channel biosignal amplifier. Thanks to the power of Due, a 32-bit powerful microcontroller, with  it lots of local memory and fast processing speeds, you will be able to develop incredible applications.

The Signalino Board can be used to sample brain activity (EEG), muscle activity (EMG), and heart activity (EKG). The board communicates wirelessly to a computer via a cheap HC-06 BT module, so that you mgh communicate your project with any BT device. 

If you are only interested in using the board for research, and you don't want programming, no problem. Download SCIGNALS, a powerful but simple to use java-based chart-recorder that we have developed, plug your Due+Signalino in a free USB port, and start recording!. 

The board come pre-loaded with the latest firmware, making signalino accessible to researchers and developers with little to no hardware experience.

This kit come with 8 electrodes. If you need more (and you know that you will...) you can purchase some in our shop. And many other things!

This kit includes:
- (x1) Signalino 
- (x1) Header pin to touch proof electrode adapter
- (x8) Cup electrodes
- (x1) 6V AA battery pack (batteries not included)
- (x4) plastic feet (for board stabilization)

### Technical Specifications:

 - 8 differential, high gain, low noise input channels
 - Compatible with active and passive electrodes
 - Texas Instruments ADS1299 ADC (link to datasheet)
 - 24-bit channel data resolution
 - 1 kHz sampling frequency 
 - Programmable gain: 1, 2, 4, 6, 8, 12, 24
 - 3.3V digital operating voltage
 - +/-2.5V analog operating voltage
 - ~3.3-6V input voltage
 - 5 GPIO pins, 3 of which can be Analog

![article-img](/img/blog/0001/signalino_prototipo_600.jpg)


###### ***Disclaimer***\
*The Signalino board is not a medical device nor is it intended for medical diagnosis and provided to you “as is,” and we make no express or implied warranties whatsoever with respect to its functionality, operability, or use, including, without limitation, any implied warranties, fitness for a particular purpose, or infringement. We expressly disclaim any liability whatsoever for any direct, indirect, consequential, incidental or special damages, including, without limitation, lost revenues, lost profits, losses resulting from business interruption or loss of data, regardless of the form of action or legal theory under which the liability may be asserted, even if advised of the possibility of such damages. This evaluation board/kit is intended for use for **ENGINEERING DEVELOPMENT, DEMONSTRATION OR EVALUATION PURPOSES ONLY** and is not considered  to be finished end-product fit for general consumer use. Persons handling the product must have electronics training and observe good engineering practice standards. As such the goods being provided are not intended to be complete in terms of required design-, marketing-, and/or manufacturing related protective considerations, including product safety and environmental measures typically found in the products that incorporte such semiconductor components or circuit boards. This evaluation board/kit does not fall within the scope of the European Union directives regarding electromagnetic compatibility, FCC, CE or UL and therefore may not meet the technical requirements of these directives or other related documents.*

### Read next
[Memboost, improve learning by improving sleep](/blog/enhancing-memory-memboost/)
