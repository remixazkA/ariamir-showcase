# Hardware Compatibility Lab

Ariamir's Hardware Compatibility Lab is the public-facing framework for validating local AI workloads on real components.

## Reference workstation

| Component | Reference configuration |
| --- | --- |
| CPU | Intel Core i7-12700KF |
| GPU | NVIDIA GeForce RTX 4080 16 GB |
| System memory | 32 GB |
| Platform | Windows x64 |

This configuration is a baseline, not a minimum requirement.

## What the lab measures

Depending on the component and workload, reports may include installation and driver compatibility, model/backend compatibility, throughput, latency, time-to-first-output, VRAM/RAM consumption, sustained-load behaviour, thermal and power observations when instrumentation is available, failure/recovery behaviour and workload suitability.

## Component classes

The lab is intended to cover GPUs and AI accelerators, FPGAs and heterogeneous compute devices, CPUs and platform changes, system memory, SSD/NVMe and storage pipelines, networking, power/cooling, chassis/workstation ergonomics and capture/media hardware where relevant.

## Partner hardware policy

Receiving hardware does not guarantee a positive result or public endorsement. Ariamir separates:

1. **Compatibility** — does it work?
2. **Performance** — how does it behave under a defined workload?
3. **Suitability** — where does it make engineering sense?
4. **Editorial acknowledgement** — what may be publicly attributed to the vendor?

Partner-provided units should be identified as such when a public result is published, unless an agreed embargo applies.

## Reproducibility

Published benchmark claims should include enough non-proprietary information to reproduce the measurement: hardware, driver/backend versions, model identifier where licensing allows, workload parameters, run count and metric definition.
