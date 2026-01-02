---
title: AR and AI-based Health Self-Screening
---

# AR and AI-based Health Self-Screening

{%
  include figure.html
  image="images/project/banner_1_cropped.png"
  caption="Overview of the AI and AR-based stethoscope self-screening platform."
%}

The stethoscope is one of the most important diagnostic tools used by healthcare professionals, through a process called auscultation ("listening to the body"), to screen patients for abnormalities of the heart and lungs. While there are digital stethoscopes on the market which ease this process, it still takes years of training to properly use these devices to listen for abnormal sounds within the body. We present ARSteth, an intelligent stethoscope platform that improves the accessibility of stethoscopes for the general population, allowing anyone to perform auscultation in the comfort of their own homes. Our platform utilizes a combination of augmented reality (AR), acoustic intelligence, and human-machine interaction to dynamically guide users on where to place the stethoscope on different parts of the body (auscultation points), through visual and audio cues.

{%
  include figure.html
  image="images/project/projection_arsteth.png"
  caption="Processing from camera to detect coarse-grained auscultation locations, much like how doctors use their eyes."
%}

First, we leverage computer vision techniques to identify a rough estimate of the proper auscultation points on an individual, much like how a physician leverages his or her eyes.

{%
  include figure.html
  image="images/project/murmur_2_arsteth.png"
  caption="Audio processing from stethoscope to search for fine-grained auscultation locations, much like how doctors use their ears."
%}

Next, our AR overlay guides the user to place the stethoscope on his or her body. In this phase, we analyze audio signals from the stethoscope to guide users on where to move such that the signal-to-noise ratio of the heart beat and the confidence of our heart murmur detector is maximized. This process is similar to how physicians fine-tune the location of the stethoscope using their ears.

{% include section.html %}

## Publications

{% include list.html data="citations" component="citation" style="rich" filters="group: arsteth_cu" %}

