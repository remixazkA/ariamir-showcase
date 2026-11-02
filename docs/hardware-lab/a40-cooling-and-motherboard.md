# A40 cooling and motherboard observations

**Hardware Compatibility Lab · 2 November 2026**

## Summary

These observations explore three ways to direct air through one passively cooled NVIDIA A40 and compare the same system before and after a motherboard change. In the latter comparison, the printed duct was also sealed with tape, so the individual effects cannot be separated. The sealed configuration had a lower observed temperature at similar power; generation rates were close in these particular runs. These are single-pass engineering observations, not a published benchmark or a general ranking.

## Equipment and conditions

- NVIDIA A40, 48 GB, passive heatsink; 300 W power limit; NVIDIA driver 616.92. Intel Core i7-12700KF platform.
- The same Arctic S4028-15K fans ran at approximately 10,500 RPM for the cooling comparison. The printed adapter was made by [MB Custom Things](https://www.etsy.com/shop/MBCustomThings).
- Recorded ambient temperature was approximately 15 °C for the home-made duct and 14 °C for the printed adapter tests and the motherboard comparison.
- Before the motherboard change the printed adapter was unsealed; afterwards its air leaks were sealed with tape. Both changes occurred between measurements.

## Method

The home-made duct was tested in power steps, including approximately 10 minutes near 300 W. The printed adapter was tested before and after sealing with an approximately eight-minute continuous single-request stress workload near 283 W. The plots show the recorded temperature and power against elapsed time; the home-made run has a different power and duration, so the curves are not an equal-power comparison.

For the motherboard comparison, GPU telemetry was sampled approximately once per second. The same workload sequence included idle without and with the model loaded, a single request, a 25,554-token long prompt, and approximately 10 minutes of six concurrent requests. A separate approximately eight-minute continuous single-request stress run followed. Throughput is generated or prompt tokens divided by the relevant elapsed processing time, as labelled; the six-request figure is aggregate throughput. The workload used a quantized 27B model with an 8-bit cache; exact model and software details are withheld. No prompts or private data are published.

The charts sample the recorded time series for legibility, with each phase aligned to its own first sample. They can be regenerated from the source dataset with the Node scripts in `tools/hardware-lab/`; the source data is not part of this public repository.

## Cooling results

The following estimates normalize the original report's measurements to **283.4 W and 14 °C**, using its 0.151 °C/W adjustment for the home-made duct. They are calculated estimates, not three direct measurements at identical conditions.

| Solution | Estimated temperature at common conditions |
| --- | ---: |
| Home-made duct | 73.1 °C |
| Printed adapter, unsealed | 76.6 °C |
| Printed adapter, sealed with tape | 72.2 °C |

In the measured printed-adapter stress runs, steady-state temperatures were 76.8 °C unsealed and 72.0 °C sealed, at 284.5 W and 282.3 W respectively. The report also observed roughly 2 dB less noise after sealing; this is an observation for this setup, not a standardized acoustic rating. The motherboard also changed between these runs.

![Cooling temperature over time](../../media/hardware-lab/a40/cooling-temperature.svg)
![Cooling power over time](../../media/hardware-lab/a40/cooling-power.svg)

## Motherboard and sealing: before and after

| Measurement | Before | After |
| --- | ---: | ---: |
| Idle unloaded: average temperature / power | 25.1 °C / 14.1 W | 24.0 °C / 14.1 W |
| Idle loaded: average temperature / power | 33.2 °C / 73.6 W | 31.6 °C / 72.6 W |
| Single request: peak temperature | 69 °C | 66 °C |
| Long prompt: peak temperature | 74 °C | 70 °C |
| Six requests: steady-state average temperature / power | 65.9 °C / 219.6 W | 61.9 °C / 216.6 W |
| Single-request stress: steady-state average temperature / power | 77.2 °C / 284.5 W | 72.3 °C / 282.2 W |
| Single-request stress: peak temperature | 79 °C | 74 °C |

| Throughput (tokens/s) | Before | After |
| --- | ---: | ---: |
| Single request: generation | 53.3 | 53.5 |
| Single request: prompt processing | 721.6 | 727.2 |
| Long prompt: prompt processing | 971.6 | 975.6 |
| Six concurrent requests: aggregate generation | 96.4 | 96.4 |
| Continuous single-request stress: generation per request | 49.9 | 50.2 |

![Before and after throughput](../../media/hardware-lab/a40/throughput.svg)

### Time series by workload

Each pair shows temperature and power separately. Time zero is the first telemetry sample in that phase, rather than a synchronized wall clock.

**Idle, model unloaded**

![Idle unloaded temperature](../../media/hardware-lab/a40/motherboard-reposo-descargado-temperature.svg)
![Idle unloaded power](../../media/hardware-lab/a40/motherboard-reposo-descargado-power.svg)

**Idle, model loaded**

![Idle loaded temperature](../../media/hardware-lab/a40/motherboard-reposo-cargado-temperature.svg)
![Idle loaded power](../../media/hardware-lab/a40/motherboard-reposo-cargado-power.svg)

**Single request**

![Single request temperature](../../media/hardware-lab/a40/motherboard-un-hilo-temperature.svg)
![Single request power](../../media/hardware-lab/a40/motherboard-un-hilo-power.svg)

**Long prompt**

![Long prompt temperature](../../media/hardware-lab/a40/motherboard-lectura-larga-temperature.svg)
![Long prompt power](../../media/hardware-lab/a40/motherboard-lectura-larga-power.svg)

**Sustained six-request workload**

![Six-request temperature](../../media/hardware-lab/a40/motherboard-sostenido-temperature.svg)
![Six-request power](../../media/hardware-lab/a40/motherboard-sostenido-power.svg)

**Continuous single-request stress**

![Stress temperature](../../media/hardware-lab/a40/motherboard-estres-temperature.svg)
![Stress power](../../media/hardware-lab/a40/motherboard-estres-power.svg)

## Photographs

The following views document the physical arrangements; the photographs do not establish performance on their own.

| Home-made duct | Installed home-made duct |
| --- | --- |
| ![Home-made duct outside the system](../../media/hardware-lab/a40/photos/casera-fuera.jpg) | ![Home-made duct installed](../../media/hardware-lab/a40/photos/casera-instalada.jpg) |

| Home-made duct joint | Printed adapter detail |
| --- | --- |
| ![Home-made duct joint](../../media/hardware-lab/a40/photos/casera-union.jpg) | ![Printed adapter detail](../../media/hardware-lab/a40/photos/impreso-detalle.jpg) |

| Printed adapter installed | Tape seal detail |
| --- | --- |
| ![Printed adapter installed](../../media/hardware-lab/a40/photos/impreso-instalado.jpg) | ![Tape seal detail](../../media/hardware-lab/a40/photos/cinta-detalle.jpg) |

![Side view of sealed adapter](../../media/hardware-lab/a40/photos/cinta-lateral.jpg)

## Limits and credits

Each configuration represents a single pass on one card, with no independent repetitions or uncertainty estimates. Ambient conditions, load shape and initial temperature matter. The home-made test differed in ambient temperature and power, and normalization depends on an estimated slope. The motherboard and duct seal changed together. The recorded fan noise is not a controlled acoustic study. These observations are not a published benchmark; repeated runs and a fully disclosable workload would be needed for reproducibility and broader claims.

The 3D-printed adapter is by MB Custom Things, listed as a technology collaborator in the [partner notes](../../partners/README.md). This acknowledgement does not imply an endorsement or establish how the hardware was acquired.
