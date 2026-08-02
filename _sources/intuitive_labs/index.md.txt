---
myst:
  substitutions:
    br: |
      ```{raw} html
      <br />
      ```
---

# A Methodology for Developing Physically Intuitive Laboratories for Advanced Electrical Engineering Education

:::{toctree}
:maxdepth: 1
:hidden:

data_conversion/index.md
software_defined_radio/index.md
power_electronics/index.md
other_electronic_topics/index.md
other_physics/index.md
medical_physiological/index.md
other_matter/index.md
:::

A starting point for a(n) (e)book / survey / other on developing hands-on experiments for advanced electrical engineering topics and tangentially related subjects.

Why? Well, I've been in the industry for almost a quarter of a century, touching on not all (which is impossible), but many, analog, digital, and mixed signal topics, applications, products, test methods, etc. And it's thoroughly enjoyable, and somewhat addictive.

My own life has been punctuated with an eclectic collection of educational projects, kits, experiments, and associated trauma:

- Getting Started in Electronics, Forrest Mims III, 1983. Still available, and still holds up. About the only thing that is truly obsolete is the section on unijunction transistors. I built many a project from this book, and to this day, picture smiley faces on protons and electrons.

- Breadboards and 555 timers. I truly have a love-hate relationship with the Forrest Mims Engineers Notebooks. First, Breadboards suck, no doubt about it. Second, while the 555 is truly a legendary device and a rich playground for all sorts of experimentation, almost all of the schematics you'll find have a somewhat ambiguous symbol:

  - A rectangle with pins arranged logically, with numbers, but no functional pin name.
  - A rectangle with pin names (threshold, trigger, output, etc.)... quite a bit better.
  - Worst of all - a rectangle with pins arranged as they are on the physical device, with numbers, and no functional names. This is the default LTspice symbol and it drives me bonkers.
  - BEST of all - a rectangle with an internal block diagram, showing the resistor divider, comparators, R-S flip-flop, output driver, discharge driver. I proposed this to the LTspice forum, let's see if it gets upstreamed :)

- Radio Shack N-in-1 spring terminal kits. My first was the Solar Power one, circa early 1980s. Changed my life.

- Radio Shack Microcomputer Trainer. A no-kidding 4-bit processor!

- Bell Labs Solar Power kit from 1962 that I picked up at a yard sale. Oh boy, the retroactive trauma. This kit was phenominal! (And phenominally dangerous.) It had a silicon wafer, a nichrome heater coil, doping chemicals, and... a sheet of asbestos to construct a little diffusion oven! IF I would have actually built the darn thing and followed the directions, it would have put me a decade ahead in my electrical engineering education. But alas, I was a wee pyromaniac, and ended up burning the chemicals and the rest of the materials got scattered about and lost. (I hope that asbestos ended up safely disposed of.)
  - Dr. David Parent has the modern equivalent of this in his [**Microscale Process Engineering Laboratory**](https://www.sjsu.edu/mpel/).

- Extraordinarily dangerous chemistry sets from the 1960s and 1970s. Many from Gilbert, take a look at the [**Gilbert Chemistry Sets**](https://www.acghs.org/?page_id=4310) at the A.C. Gilbert Heritage Society.

So what can I add to the conversation? Punchline first: The hands-on experience, connecting theory to simple, low-cost experiments that you can actually run on your lab bench, desk, or kitchen table.

Also - "Hybrid Techniques". One of the many fun aspects of my job is that I get to explore lots of strange and creative circuits.

- Correlated Double sampling and AC excitation (LTC2415 datasheet, AN96)
- Transparent, cotinuous low-noise gain and offset calibration from noisy calibration readings (AN112)
- Multitone narrow-band detection (FTC colorimeter)

I'm not an expert in any one particular field - DSP, IC design, matierial science, analog filter design, computer science, RF/microwave, EMI/EMC, power, etc.\*\*, but somehow I've managed to stay employed by "connecting these dots" - making sure all of these disciplines are properly applied to designs so customers can get stuff released. Add to this my "layered" experiencec - it's not just helping tier-1 "strategic and key" customers - it's designing and releaing evaluation boards, conceiving and delivering internal training sessions, onboarding new college graduates, developing university-oriented lab exercises, and if you go far enough back, presenting science topics to all ages, back to kindergarten and ealriler.

Throughout all of these, there has been a common thread of trying to make things as interactive, intuitive, and interesting as possible. I've found that the bar for an effective hands-on activity is extraordinarily low - you just have to have some nonzero physical representation of a concept in your learner's hands to augment what you're saying, what you've given as reading material, and what you're presenting on screen. (We'll very rapidly get to examples below...)

**References for Inspiration**

One of the inspirations for this is effort is this dissertation:

[**The ASPEN platform : tools for mixed signal electronics, digital signal processing, and biomedical electronics**](https://purl.stanford.edu/nq977kw3386) William Esposito, 2018.

It's a REALLY nice collection of, well, see the title.

And another:

Wernsing, G. (2024). [**Modernizing Undergraduate Software-Defined Radio Education**](https://digital.wpi.edu/concern/etds/gx41mp11n). Worcester Polytechnic Institute. ([PDF](https://digital.wpi.edu/downloads/73666903m))

Another is Dr. David S. Ricketts':

[**Advanced analog IC and Data Converter Course lectures**](https://rickettslab.org/adc/).

(Also see his "Rabbit Radar!")

An absolutely epic project by Dr. Gregory Charvat, the Coffee Can Radar!!!:

[**Build a Small Radar System Capable of Sensing Range, Doppler, and Synthetic Aperture Radar Imaging**](https://ocw.mit.edu/courses/res-ll-003-build-a-small-radar-system-capable-of-sensing-range-doppler-and-synthetic-aperture-radar-imaging-january-iap-2011/)

And of course, one of the classics, Art of Electronics by Horowitz and Hill!

[**Art of Electronics Homepage**](https://artofelectronics.net/)

:::{note}
This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) —
Attribution, NonCommercial, ShareAlike. You are free to share and adapt this material
for non-commercial purposes, provided you give appropriate credit and distribute any
adaptations under the same license.
:::
