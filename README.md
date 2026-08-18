# Lee Newton

**MOASAS — Modular Optics And Sensor Array System**

An autonomous multi-sensor field platform. Optical, thermal, acoustic,
environmental and positional sensors on a single compute core, with an
on-board AI layer that reads its own instruments and reports what it
finds in plain language.

### [project-moasas.github.io/moasas-site](https://project-moasas.github.io/moasas-site/)

---

### One body, many missions

The same array has been pointed at presence monitoring, wildlife
observation, perimeter security and mechanical health baselines — with
no rebuild between them.

Every sensor runs as its own process and publishes to a shared JSON
contract. Add a peripheral and its history becomes queryable by the AI
layer the moment it writes its file; nothing is imported into the web
application itself.

### Instrumentation

| Subsystem | Hardware |
|---|---|
| Compute | Radxa Rock 5B+ · Ubuntu · NVMe |
| Optical | Arducam · YOLOv8 detection |
| Thermal | MLX90640 · 32 × 24 @ 8 Hz |
| Acoustic | USB microphone · YAMNet TFLite |
| Environmental | BME688 on ESP32-S2 |
| Position | BN-880 GPS |
| Pointing | ESP32 pan/tilt gimbal |
| Link | LTE · dual-radio Wi-Fi · mesh VPN |

### Status

Designed and built from scratch since October 2024. Provisional patent
filed April 2026. Currently running unattended at a remote site over
cellular, with an event-gated capture pipeline, nightly archive offload,
and a tool-calling AI layer that answers questions about its own sensor
history.

### Contact

Through the [project site](https://project-moasas.github.io/moasas-site/#contact).
