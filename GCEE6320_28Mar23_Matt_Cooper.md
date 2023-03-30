---
marp: true
theme: gaia
class: 
  - invert
author: Matt Cooper
size: 4:3
paginate: true
style: |
  h1 {
    font-size: 36px;
  }
  h2 {
    font-size: 36px;
  }
  p {
    font-size: 16px;
  }
  li {
    font-size: 26px;
  }
  li li {
    font-size: 24px;
  }
  img[alt~="center"] {
    display: block;
    margin: 0 auto;
    max-width: 100%;
    max-height: 50%;
    object-fit: contain;
  }
  small-text {
    font-size: 8px;
  }
  bottom-text {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    text-align: center;
  }
---

<!-- slides_GCEE6320_28Mar23_Matt_Cooper -->

<!-- _class: lead invert --> # center justify this slide
<!-- _footer: "28 March 2023" --> # add a footer to this slide

# High-Latitude Hydroclimatology: Modeling the Cryosphere

Matt Cooper
Pacific Northwest National Laboratory
28 March 2023
matt.cooper@pnnl.gov

![center](./img/A_Snapshot_of_Sea_Ice.jpg)
<!-- ![w:400px h:auto](A_Snapshot_of_Sea_Ice.jpg) -->

<!-- <p class="small-text">Some smaller text at the footer of the page.</p> -->

---

## Importance of High-Latitude Hydroclimatology <!-- fit -->

<!-- use this to scope a style to one slide -->
<style scoped> li {font-size: 24px} </style>

<!-- ![bg right](A_Snapshot_of_Sea_Ice.jpg) -->
<!-- ![bg](A_Snapshot_of_Sea_Ice.jpg) -->

- Why do polar regions play a significant role in global climate?
    - The high albedo of snow and ice.
    - The large amount of freshwater stored in glaciers.
    - The large amount of carbon stored in permafrost.

![center w:650px h:auto](./img/A_Snapshot_of_Sea_Ice.jpg)

<!-- In this image you can see at least three distinct features of the high latitude regions: snow covered sea ice, the greenland ice sheet, and vast expanses of tundra underlain by permafrost -->

---

## Importance of High-Latitude Hydroclimatology <!-- fit -->

<!-- use this to scope a style to one slide -->
<style scoped> li {font-size: 24px} </style>

- This lecture:
    - **The high albedo of snow and ice.**
    - **The large amount of carbon stored in permafrost.**
- Next lecture:
    - The large amount of freshwater stored in glaciers.    

![center w:650px h:auto](./img/A_Snapshot_of_Sea_Ice.jpg)

---

## Learning Outcomes

- Understand the role of the cryosphere in the climate system.
- Understand polar amplification.
- Understand why sub-grid scale parameterizations are used.

---

## The High-Latitude Cryosphere: Sea Ice and Polar Snow

- Sea ice and polar snow influence global climate by reflecting sunlight, and acting as insulators that prevent heat exchange between the ocean and the atmosphere.
- Snow accumulation and melt affect the mass balance of polar ice sheets, which in turn influence global sea levels.

![center w:500px h:auto](./img/A_Snapshot_of_Sea_Ice.jpg)

---

## High-latitude regions are especially sensitive to climate change <!-- fit -->

-  Why do high latitude regions experience more pronounced warming than other areas?
    - **Snow and ice reflect _more_ solar radiation than other surfaces.**

![center w:500 h:auto](./img/weathering_crust.jpg)

---

## High-latitude regions are especially sensitive to climate change <!-- fit -->

-  Why do high latitude regions experience more pronounced warming than other areas?
    - _Snow and ice reflect _more_ solar radiation than other surfaces._
        - **As earth warms, snow cover decreases and absorbed solar radiation increases, which causes more warming, more snow melt, and more absorption of solar radiation, leading to a positive feedback loop.**

![center w:400 h:auto](./img/albedo-feedback.png)

---

![bg](https://upload.wikimedia.org/wikipedia/commons/6/6f/Arctic_Sea_Ice_Shrinks_To_New_Low_In_Satellite_Era_%287873358708%29.jpg)

<!-- This image shows the lowest observed sea ice extent on Aug 26, 2012. As sea ice extent shrinks, more water is exposed, which absorbs more heat, leading to more warming, and less sea ice. -->

<p style=" position: absolute; bottom: 0; left: 0; width: 100%; text-align: center;">NASA Goddard Space Flight Center from Greenbelt, MD, USA, Public domain, via Wikimedia Commons</p>

---

![center](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/20220726_Feedbacks_affecting_global_warming_and_climate_change_-_block_diagram.svg/1024px-20220726_Feedbacks_affecting_global_warming_and_climate_change_-_block_diagram.svg.png)

<p class="small-text">RCraig09, CC BY-SA 4.0, via Wikimedia Commons</p>

<!-- in addition to the ice albedo feedback, there are two other positive feedbacks related to the Cryosphere: changes in water vapor/clouds, and melting permafrost -->

---

## Polar Amplification

<!-- from the prior version -->
- Polar amplification refers to the increased rate of warming in the Arctic and Antarctic compared to the global average.
- This phenomenon is caused by various positive feedback mechanisms, such as the ice-albedo feedback and the release of greenhouse gases from thawing permafrost.

![center w:500 h:auto](https://upload.wikimedia.org/wikipedia/commons/b/b6/Methane_Releases_-_East_Siberian_Arctic_Shelf_%284416688271%29.jpg)

<!-- these mechanisms are referred to as polar amplification -->
<!-- we wont discuss water vapor, clouds, or lapse rate feedback, but if students are interested, the polar atmosphere can often have a lower lapse rate leading to less efficient longwave cooling from the TOA -->

---

## Polar Amplification

- High-latitude regions warm faster than the global average
    - Arctic: 2.5°C
    - Antarctic: 1.5°C
    - Global: 1.1°C
- Factors: Ice-albedo feedback, changes in atmospheric and oceanic circulation, and increased greenhouse gases.


![center w:400px h:auto](https://upload.wikimedia.org/wikipedia/commons/f/f3/GISS_temperature_2000-09.png)

<p class="small-text">https://commons.wikimedia.org/wiki/File:GISS_temperature_2000-09.png</p>

<!-- 
- Polar amplification is the phenomenon where high-latitude regions warm faster than the global average due to various feedback mechanisms.
- Key factors contributing to polar amplification include ice-albedo feedback, changes in atmospheric and oceanic circulation, and increased greenhouse gas concentrations. 
-->

---

## Question: why are the northern latitudes warming more than the southern latitudes?

![center ](https://upload.wikimedia.org/wikipedia/commons/f/f3/GISS_temperature_2000-09.png)

<!-- Question: Why is the north so much warmer than south? -->

---

## Global Climate Models for Hydroclimatology

- Climate models are essential tools for studying and predicting hydroclimatic processes in high-latitude regions.
- Accurately representing high-latitude processes in climate models is challenging due to the complex interactions between the atmosphere, ocean, and cryosphere.

![center w:600px h:auto](./img/Global_Climate_Model_merged.png)

---

<!-- _backgroundColor: white -->

![bg w:100%](./img/USGS_WaterCycle_English_ONLINE_20221013_cropped.png)

---

## Permafrost Hydrology

- Permafrost is permanently frozen ground, and it affects the storage and movement of water in high-latitude regions.
- Thawing permafrost can release significant amounts of carbon dioxide and methane, both potent greenhouse gases, exacerbating climate change (permafrost-carbon feedback).

![center w:800px h:auto](./img/polygonal_ground.png)

---

## Permafrost Hydrology

- Permafrost stores large amounts of carbon and water.
- Thawing permafrost affects hydrology, ecosystems, and infrastructure.

![bg right w:450px h:auto](./img/active_layer_diagram.png)

<p class="small-text">diagram: Kurylyk et al (2014) ESR</p>

---

## Arctic methane emissions

![center w:700 h:auto](https://upload.wikimedia.org/wikipedia/commons/8/8d/CH4.BRW.Monthly.png)

---

## Permafrost Hydrology

- Permafrost is permanently frozen ground, and it affects the storage and movement of water in high-latitude regions.
- Thawing permafrost can release significant amounts of carbon dioxide and methane, both potent greenhouse gases, exacerbating climate change (permafrost-carbon feedback).

![center w:800px h:auto](./img/polygonal_ground.png)

---

## Polygonal ground

![bg](https://upload.wikimedia.org/wikipedia/commons/7/73/Polygonal_Ground_in_Nunavut_in_Canada_-_Aerial_photo.jpg)

---

## Polygonal ground

![bg](https://upload.wikimedia.org/wikipedia/commons/b/b2/Frost_polygons_in_ground_%28Gardner_Lake_trailhead%2C_Beartooth_Mountains%2C_Wyoming%2C_USA%29_11.jpg)

---

## Permafrost Hydrology

- Thawing permafrost affects hydrology, ecosystems, and infrastructure

![center w:1000px h:auto](./img/polygonal_ground.png)

<p class="small-text">image: Ethan Coon, AMANZI-ATS</p>

---

## Sub-grid parameterization

- How do we represent this complexity in models? 
- Answer: sub-grid parameterizations

![center w:680px h:auto](./img/subgrid_param_cesm.png)

<p class="small-text">image: https://www2.cesm.ucar.edu/working_groups/Atmosphere/parameterizations/</p>

---

## Sub-grid parameterization

<!-- _backgroundColor: white -->
<!-- _color: black -->

![bg w:900](./img/subgrid_param_cesm_annotated.png)

---

## Case Study: Representing permafrost in models <!-- fit -->

<!-- _backgroundColor: white -->
<!-- _color: black -->

![center](https://upload.wikimedia.org/wikipedia/commons/b/b2/Frost_polygons_in_ground_%28Gardner_Lake_trailhead%2C_Beartooth_Mountains%2C_Wyoming%2C_USA%29_11.jpg)

---

<!-- _backgroundColor: white -->
<!-- _color: black -->

![center w:800 h:auto](./img/ats-mosart-diagram.png)

---

<!-- _backgroundColor: white -->
<!-- _color: black -->

- Observations show an earlier peak in spring
- Observations show fewer peaks in late summer

![center w:800 h:auto](./img/ats-mosart-usgs-2.png)

---

## Sub-grid parameterization of soil ice content

<!-- _backgroundColor: white -->
<!-- _color: black -->

- Represent the effect of soil ice content on lateral flow with parameter $\Theta_{ice}$

![center w:800 h:auto](./img/elm-subgrid.png)

---

## Learning outcomes

- Understand the role of the cryosphere in the climate system.
- Understand polar amplification.
- Understand why sub-grid scale parameterizations are used.

---

## Learning outcomes

- Understand the role of the cryosphere in the climate system.
    - **High albedo of snow and ice.**
    - **Large amount of carbon stored in permafrost.**

---

## Learning outcomes

- _Understand the role of the cryosphere in the climate system._
- **Understand polar amplification.**
    - **The Arctic warming faster than the rest of the globe due to positive feedbacks in the climate system.**
    - **As the Arctic warms, snow cover declines, leading to more heat absorption, more warming, and more snow melt.**
    - **As the Arctic warms, permafrost melts, releasing carbon, leading to more warming, and more permafrost melt.**

---

## Learning outcomes

- _Understand the role of the cryosphere in the climate system._
- _Understand polar amplification._
- **Understand why sub-grid scale parameterizations are used.**
    - **Climate processes are complex, and it is not possible to represent them all in a climate model.**
    - **Sub-grid parameterizations capture the effects of processes that are not explicitly resolved in the model.**

---

## Recap and Takeaway Messages

- High-latitude hydroclimatology is critical for understanding global climate change.
- Climate models are essential tools for studying hydroclimatic processes.
- Polar amplification, sea ice, permafrost, and freshwater inputs play key roles.
- The accuracy of climate models is challenged by complex interactions between different components of the Earth system, and the necessity of representing them with sub-grid parameterizations.

--- 

## Questions?

![bg](./img/A_Snapshot_of_Sea_Ice.jpg)


---

![bg](https://upload.wikimedia.org/wikipedia/commons/thumb/7/75/Oblique_rays.svg/1024px-Oblique_rays.svg.png)
