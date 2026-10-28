# Hardware Compatibility Lab

Ariamir's Hardware Compatibility Lab is the public-facing framework for validating local AI workloads on real components.

## Reference workstation

| Component | Reference configuration |
| --- | --- |
| CPU | Intel Core i7-12700KF |
| GPU | NVIDIA GeForce RTX 4080 16 GB |
| System memory | 32 GB |
| Platform | Windows 11 x64 |

This configuration is a baseline, not a minimum requirement. Development builds currently target Windows 11.

## Lab inference server

Alongside the reference workstation, the lab runs a local inference server with an **NVIDIA A40 (48 GB)**, used to test parallel agents, long contexts and connections from a second Windows PC through a keyed gateway.

### Early observations (28 October 2026)

Single short runs on the same model file, **Qwen3.8 27B (Q4_K_M weights, 8-bit KV cache)**. They are indicative only: a repeated, published benchmark is still pending.

| Measurement | Ollama 0.34.2 | llama.cpp server b11951 with speculative decoding (MTP) |
| --- | --- | --- |
| Generation, one request | 85 tokens/s | 87.6 tokens/s |
| Six requests at once, total | 70 tokens/s (processed one after another) | 182 tokens/s |
| Prompt processing, ~39K-token prompt | 861 tokens/s | 902 tokens/s |
| Repeated shared prefix | 1.6 s | 0.78 s |
| GPU memory | 23 GB (one request at a time) | 44.7 GB (six 96K-token contexts) |

What stood out:

- With this hybrid-architecture model, the tested Ollama version served requests one at a time, while the llama.cpp server handled six at once.
- Prompt-cache reuse for hybrid models needs the inference engine to keep context checkpoints; with them, about 99% of a repeated prefix was reused.
- Speculative decoding with the model's own multi-token-prediction heads roughly doubled generation throughput without changing the output.
- A 66,430-token prompt was processed in 85 seconds and answered correctly in a simple retrieval check.

## AMD Radeon on Windows

Support for AMD Radeon graphics is in development, starting with Vulkan. Validation on a real **AMD Radeon RX 9070 XT** is planned with an external tester; results will be published here once they are available.

Partner-provided hardware is added to this page once it is installed and tested; see [current partners](../partners/README.md#current-partners).

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
