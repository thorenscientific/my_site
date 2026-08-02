---
myst:
  substitutions:
    br: |
      ```{raw} html
      <br />
      ```
---

# Software-Defined Radio

```{rubric} Software-Defined Radio
```

As a source of inspiration, it does not get much better than PySDR.org: {{ br }}
[PySDR: A Guide to SDR and DSP using Python](https://pysdr.org/)

So I'm no real expert in SDR, but there are a few pretty interesting concepts I've brought to life in fun side projects. In 2021 I did a talk at the GNU Radio Conference on "Python for the Rest of Us". In it I buitl what I refer to as "The world's silliest AM to FM translator", using an ADALM2000 to digitize the 455 kHz IF of an Elenco AM radio kit (Yup, building the AM radio was part of this :) ) I use GNU Radio to demodulate the audio, then re-modulate as FM, and send to an ADALM-Pluto.

(Take a peek around 50:55)

```{raw} html
<iframe width="560" height="315" src="https://www.youtube.com/embed/cO5sBarLiVk" title="Python for the Rest of Us" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
```

```{rubric} Crystal Radios
```

Yup, you bet! Build a crystal radio using a ceral box, and tune it up using the ADALM2000 network analyzer.

```{rubric} Other References
```

Field-Expedient SDR by Paul Clark and David Clark

Software Defined Radio for Engineers by Travis Collins, Robin Getz, Di Pu, Alexander Wyglinski

% # define a hard line break for HTML
