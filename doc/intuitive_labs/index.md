---
myst:
  substitutions:
    br: |
      ```{raw} html
      <br />
      ```
---

# A Methodology for Developing Physically Intuitive Laboratories for Advanced Electrical Engineering Education

```{eval-rst}
.. toctree::
   :maxdepth: 1
   :hidden:

   data_conversion/index.md
   software_defined_radio/index.md
   power_electronics/index.md
   other_electronic_topics/index.md
   other_physics/index.md
   medical_physiological/index.md
```

A starting point for a(n) (e)book / survey / other on various things practical mixed signal.

Why? Well, I've been in the industry for almost a quarter of a century, touching on not all (which is impossible), but many, analog, digital, and mixed signal topics, applications, products, test methods, etc. And it's thoroughly enjoyable, and somewhat addictive.

So what can I add to the conversation? Punchline first: The hands-on experience, connecting theory to simple, low-cost experiments that you can actually run on your lab bench, desk, or kitchen table.

Also - "Hybrid Techniques". One of the many fun aspects of my job is that I get to explore lots of strange and creative circuits.

> - Correlated Double sampling and AC excitation (LTC2415 datasheet, AN96)
> - Transparent, cotinuous low-noise gain and offset calibration from noisy calibration readings (AN112)
> - Multitone narrow-band detection (FTC colorimeter)

I'm not an expert in any one particular field - DSP, IC design, matierial science, analog filter design, computer science, RF/microwave, EMI/EMC, power, etc.\*\*, but somehow I've managed to stay employed by "connecting these dots" - making sure all of these disciplines are properly applied to designs so customers can get stuff released. Add to this my "layered" experiencec - it's not just helping tier-1 "strategic and key" customers - it's designing and releaing evaluation boards, conceiving and delivering internal training sessions, onboarding new college graduates, developing university-oriented lab exercises, and if you go far enough back, presenting science topics to all ages, back to kindergarten and ealriler.

Throughout all of these, there has been a common thread of trying to make things as interactive, intuitive, and interesting as possible. I've found that the bar for an effective hands-on activity is extraordinarily low - you just have to have some nonzero physical representation of a concept in your learner's hands to augment what you're saying, what you've given as reading material, and what you're presenting on screen. (We'll very rapidly get to examples below...)

```{rubric} References for Inspiration
```

One of the inspirations for this is effort is this dissertation: {{ br }}
[The ASPEN platform : tools for mixed signal electronics, digital signal processing, and biomedical electronics](https://purl.stanford.edu/nq977kw3386) William Esposito, 2018. It's a REALLY nice collection of, well, see the title.

And another: {{ br }}
Wernsing, G. (2024). [Modernizing Undergraduate Software-Defined Radio Education](https://digital.wpi.edu/concern/etds/gx41mp11n). Worcester Polytechnic Institute. ([PDF](https://digital.wpi.edu/downloads/73666903m))

Another is Dr. David S. Ricketts' [Advanced analog IC and Data Converter Course lectures](https://rickettslab.org/adc/). {{ br }}
(Also see his "Rabbit Radar!")

And of course, one of the classics, Art of Electronics by Horowitz and Hill!

[Art of Electronics Homepage](https://artofelectronics.net/)

:::{note}
This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) —
Attribution, NonCommercial, ShareAlike. You are free to share and adapt this material
for non-commercial purposes, provided you give appropriate credit and distribute any
adaptations under the same license.
:::

% # define a hard line break for HTML
