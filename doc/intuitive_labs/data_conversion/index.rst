Data Conversion and Signal Processing
======================================

Here's a blurb I wrote as one of our Active Learning exercises was turned into an Analog Dialogue article:

"Sometime in 1998, I followed a tutorial for hooking up an Analog to Digital converter to a "Basic Stamp" microcontroller. As I turned the little blue dials and watched the numbers on my (MS DOS 6.22) screen go from 0 to 4095, my jaw dropped, and something snapped in my brain - paraphrasing: "Holy F___!!** this is the coolest thing EVER!". Soon after, I quit my job, went back to UMaine for my MSEE degree, and ended up supporting that very ADC as an apps engineer at Linear Technology Corporation. 20 years later, I'm still fascinated by converting signals from analog to digital and vicey-versy.
What are these magical devices that show up everywhere - in you cell phone, your TV, your car... everywhere.?? Build one yourself! Here's a little tutorial from my colleagues and I: `ADALM2000 Activity: Analog-to-Digital Conversion <https://www.analog.com/en/resources/analog-dialogue/studentzone/studentzone-february-2022.html>`__"

This appnote is still out in the wild, I recently re-built it for nostalgia sake. ToDo: Add photo of rebuild. |br|
`BASIC Stamp II Application Notes: Serial ADC with Shiftout and Shiftin <https://www.farnell.com/datasheets/307474.pdf>`__

** "Holy Fun." (That's what I said... really.)


.. rubric:: My own stuff to expand upon

I've explored various topics to one degree or another before, so why not start with these? 

`ADC Crash Course! <https://github.com/thorenscientific/ROUS/blob/master/educational/ADC_crash_course/ADC_Crash_Course_with_output.ipynb>`__ |br|
A VERY rough start on an "ADC Crash Course", as a Jupyter Notebook. |br|
(This is a verson with saved output plots, may be out of date. Take out the "_with_output" from the URL to get the latest.)

`Using Python for Analysis and Verification of Mixed-mode Signal Chains <https://proceedings.scipy.org/articles/majora-1b6fd038-001>`__ |br|
Mark Thoren and Cristina Șuteu, Scientific Computing with Python Conference, July 2021. |br|
The one with the most current relevance is this paper from a few years back. It doesn't dive terribly deep, but links analog and digital simulation and measurement, and provides a template for other topics.

`Noise, Filters, and Mixed-Mode Signal Chains - Mark Thoren <https://www.youtube.com/watch?v=KYsf1FuKLIY>`__ (YouTube Video) |br|
Related to the above, a lecture at San Jose State with some nuggets to formalize and distill.

`Delta Sigma ADC Bridge Measurement Techniques <https://www.analog.com/media/en/technical-documentation/application-notes/an96fa.pdf>`__, Linear Technology Application Note, January 2005. |br|
Some ancient, but still relevant history.

.. rubric:: Work / Analog Devices related referenes

`Tools for Low Speed Mixed Signal System Design <https://analogdevicesinc.github.io/documentation/learning/tools_for_ls/index.html>`__ |br|
This one is mostly focused on software control of ADCs and DACs using Linux device drivers. Think of it as a "facilitator" or foundational section. But it does have a tiny bit of LTspice, some basic measurments involving a tiny bit of math, so it's not a bad place to start out. Also a great place for pointing out the distinction between industry standard software vs. bespoke / one-off.

`ADI’s Software Infrastructure for designing with ADCs, DACs, and Sensors <https://trupples.github.io/adi-documentation/learning/sw_infrastructure/index.html>`__ |br|
This is also foundational, but adds in tools for generating and analyzing signals, working with buffers of data .

Note that this is in a fork of analogdevicesinc/documentation, The future home will be `HERE <https://analogdevicesinc.github.io/documentation/learning/sw_infrastructure/index.htmltr>`__.

`"Webinar: Noise Analysis in Precision Analog Designs" <https://ez.analog.com/webinar/c/e/157>`__ |br|
Done by Scott Hunt, most excellent. (`Slide Deck <https://ez.analog.com/webinar/m/presentations/2772>`__, `Video link <https://ez.analog.com/webinar/m/recordings/2468>`__)


.. rubric:: Unsorted References

Let's start by scrubbing Analog Devices' technical books. Here's a search: |br|
`resourceTypes=Education~Technical Book <https://www.analog.com/en/search.html?resourceTypes=Education~Technical%20Book>`__


`High Speed Design Seminar, 1990 <https://www.analog.com/en/resources/technical-books/high-speed-design-seminar.html>`__ - A/D, D/A conversion

This is a good chunk of the scope I hope to cover here... circa 2001: |br|
`Mixed-Signal Design Seminar, 1991 <https://www.analog.com/en/resources/technical-books/mixed-signal-design-seminar.html>`__. Edited by Walt Kester, Analog Devices, 1991, ISBN-0-916550-08-7. |br|
(`Zip file of entire book <https://www.analog.com/media/en/training-seminars/design-handbooks/Mixed-Signal-Design-Seminar-1991/Mixed-Signal-Design-Seminar-1991.zip>`__)

From the landing page: |br|
The first Analog Device’s worldwide seminar to treat the fundamentals of data conversion for DSP applications, including Fast Fourier Transforms, Digital Filters, and DSP hardware. The material was updated and expanded in the Mixed Signal and DSP Design Techniques book published in 2000.

(From Figure 1.10 - State of the Art in ADCs - Resolution 22 bits, sampling rate 1 kSPS - HaHa!)

This is dated, of course, but covers Amplifiers, ADCs, mux considerations, distortion mechanisms, analog prototyping techniques. |br|
`Practical Analog Design Techniques, 1995 <https://www.analog.com/en/resources/technical-books/practical-analog-design-techniques.html>`__

`Mixed Signal and DSP Design Techniques, 2002 <https://www.analog.com/en/resources/technical-books/mixed_signal_dsp_design_book.html>`__ |br|
"This book covers the fundamentals of mixed-signal circuits from the viewpoint of the practicing engineer. The theory of sampled data systems, ADCs, and DACs is discussed, along with practical examples. Fast fourier transforms and digital filter fundamentals are presented in a fashion that minimizes the detailed mathematics. The book concludes with DSP hardware fundamentals, interfacing, and practical PCB layout techniques."

This is also probably a bit dated - we will sort through this for perspective: |br|
`The Data Conversion Handbook, 2005 <https://www.analog.com/en/resources/technical-books/data-conversion-handbook.html>`__, Walt Kester, ISBN 0-916550-27-3 (`Zip file of entire book <https://www.analog.com/media/en/training-seminars/design-handbooks/Data-Conversion-Handbook/analog_digital_conversion.zip>`__)

And THIS one is REALLY dated! (Thoren was -1 years old when it was published!): |br|
`Analog-Digital Conversion Handbook, 1972 <https://www.analog.com/en/resources/technical-books/analog-digital-conversion-1972.html>`__
(`Zip file of entire book <https://www.analog.com/media/en/training-seminars/design-handbooks/Analog-Digital-Conversion-1972/Analog-Digital-Conversion-Handbook-1972.zip>`__)

.. rubric:: Digital Signal Processing

An insanely interesting collection of DSP concepts, illustrated with Python: |br|
`Learning DSP Illustrated <https://dspillustrations.com/pages/index.html>`__


.. rubric:: "OG" References - Fundamental stuff

`Digital Signal Processing by Alan V. Oppenheim, Ronald W. Schafer <https://www.goodreads.com/book/show/166326.Digital_Signal_Processing>`__

`The Fast Fourier Transform and Its Applications by E. Brigham <https://www.goodreads.com/book/show/126326741-the-fast-fourier-transform-and-its-applications-prentice-hall-signal-pr>`__

`On the use of windows for harmonic analysis with the discrete Fourier transform, F.J. Harris, 1978 <https://ieeexplore.ieee.org/document/1455106>`__
(`PDF from an MIT site <https://web.mit.edu/xiphmont/Public/windows.pdf>`__)


Stream of Consciousness Brainstorm for a table of contents.

.. rubric:: Data Converter History

* Fluff chapter with some interesting architectures.
* Potentiometer servo ADC
* Kelvin-Varley Divider (don't forget Williams' references)
* DAC with external deglitcher

.. rubric:: Fundamentals of Sampled Data Systems

dt * dv/dt = dv... it's the law!

* Toolbox Items
   * Data sources and sinks
   * Analog signal sources and sinks
   * Hardware for converter testing
      * ADALM2000
      * Sound Card
      * ADALM-Pluto
      * Clock sources

.. rubric:: Analog to Digital Converters

* ADC Architectures
   * SAR (Modern, q noise lower than thermal noise)
   * RF (Beyond typical pipeline)
   * Multi-slope

* Testing ADCs
   * Overview of commercial production Testing Techniques
   * Practical techniques
   * Reference Noise: Broadband
   * Reference Noise: Amplitude Modulation
   * Reference Noise: "Noisy Wire" techique



* ADC Circuit Techniques
   * Correlated Double sampling and AC excitation (LTC2415 datasheet, AN96)
   * Transparent, cotinuous low-noise gain and offset calibration from noisy calibration readings (AN112)
   * Multitone narrow-band detection (FTC colorimeter)

.. rubric:: Digital to Analog Converters

* DAC Architectures
   * PWM DACs
   * Microcontroller PWM peripherals and their Limitations
   * Analogy to sigma-delta DACs
   * Extension to Class-D modulation

* DAC Circuit techniques
   * Settling time - the Autozero Clamplifier (Don't forget Williams appnotes)
   * Settling time - ADC techniques

* Voltage references
   * Ratiometric circuits
   * Noise reduction techniques - filtering, paralleling
* Interfacing to Data Converters
* Data Converter Support Circuitry
* Data Converter Applications
* Hardware Design Techniques


.. # define a hard line break for HTML
.. |br| raw:: html

   <br />
