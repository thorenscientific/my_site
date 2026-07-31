---
myst:
  substitutions:
    br: |
      ```{raw} html
      <br />
      ```
---

# Other Electronic Topics

```{rubric} A Wien Bridge Oscillator
```

There are a lot of things you can learn by building a Wien bridge oscillator! This one goes pretty deep - starting with a theoretical treatment of oscillators, Barkhausen criterion, LTspice simulation of a perfect oscillator, then an oscillaor with simple diode clamping to limit amplitude, but at the expense of distortion. we explore the harmonic content for symmetric an asymmetric clipping, too. Next we replace diode clamps with an incandescent bulb, just like Bill Hewlett did!

This is published as an Active Learning exercise at: {{ br }}

[Activity: The Wien Bridge Oscillator](https://developer.analog.com/docs/system-level/university/active_learning/wien_bridge_oscillator/index.html)

And here's the video to go along with it:

```{raw} html
<iframe width="560" height="315" src="https://www.youtube.com/embed/XbeZBm2lghw" title="A Low-Distortion Wien Bridge Oscillator You Can Build! (with Theory, Simulation, and Testing)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
```

{{ br }}

```{rubric} Flip-flop timing, Metastability
```

Here's a pretty deep dive into setup and hold times and metastability. We all know that violating timing on a flip flop (which could be the intput register of a SPI port) can result in data being shifted one bit in the wrong direction. But if you're right on the edge, you could end up with indeterminate behavior - metastiability where the output of the register "hangs" somewhere between logic high and logic low. There are techniquest to avoid this - synchronizer chains, special techniques when mutltiple bits need to pass bettween clock domains. But observing metastibiltity directly is annoyingly difficult! Well, in this video we build a circuit to purposely force a worst-case timing situation, and actually catch the output of a flip-flop in the act!

```{raw} html
<iframe width="560" height="315" src="https://www.youtube.com/embed/dsx4BKkhRBE" title="Flip-flop timing, my favorite interview question, and the strangest circuit I&#39;ve ever built" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
```

{{ br }}

```{rubric} Layout
```

The best four pages ever written on mixed-signal layout: {{ br }}
[Partitioning and Layout of a Mixed-Signal PCB](https://hott.shielddigitaldesign.com/pdf_files/june2001pcd_mixedsignal.pdf)

{{ br }}

Put some stuff in here regarding thermal resistance, signal integrity, power
supply decopuling, etc.

% # define a hard line break for HTML
