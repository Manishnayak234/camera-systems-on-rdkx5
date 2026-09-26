# m1-csi-inspector

RDK X5 + MIPI CSI based IMX219 camera.

> **Status: scaffold only.** The source files in this repository (`csi_inspect.c`, `Makefile`, and
> `m1-csi-inspector/README.md`) are currently empty. This README describes only what the
> repository actually contains today; every section that would require working code is marked
> **TODO** and should be filled in as the implementation lands.

---

## Overview

`m1-csi-inspector` is the first module ("m1") of a project targeting an **IMX219 image sensor**
connected over **MIPI CSI** to a **Horizon Robotics RDK X5** board. The module is named after its
single source file, `csi_inspect.c`, which is intended to be a C program built with `make`.

No capture, inspection, or processing logic has been implemented yet.

## Hardware Setup

| Component      | Details                                   |
| -------------- | ----------------------------------------- |
| Board          | Horizon Robotics RDK X5                   |
| Camera sensor  | Sony IMX219                               |
| Interface      | MIPI CSI                                  |

- **TODO:** CSI port / connector used on the RDK X5.
- **TODO:** Ribbon cable type and orientation.
- **TODO:** Any device-tree, sensor-config, or board-level settings required.

## Software Dependencies

The repository contains no code, build rules, or dependency manifests yet, so no dependencies can
be listed with certainty. Based on the file types present, building will require:

- A C compiler
- GNU Make

- **TODO:** RDK X5 OS image / BSP version.
- **TODO:** Libraries and headers used by `csi_inspect.c`.

## Repository Structure

```
.
├── README.md                  # This file
└── m1-csi-inspector/
    ├── Makefile               # Build rules (currently empty)
    ├── README.md              # Module README (currently empty)
    └── csi_inspect.c          # Module source (currently empty)
```

## Build and Run

The `Makefile` is currently empty, so there are no build targets or run commands to document yet.

```bash
cd m1-csi-inspector
# TODO: build command(s) once the Makefile defines targets
# TODO: run command and arguments once csi_inspect.c is implemented
```

## How It Works

No pipeline is implemented yet. The diagram below shows only the hardware path implied by the
project description; the software stages are placeholders.

```mermaid
flowchart LR
    A[IMX219 sensor] -->|MIPI CSI| B[RDK X5]
    B --> C["csi_inspect (TODO)"]
    C --> D["Output (TODO)"]
```

## Results

No measurements have been taken yet.

| Metric               | Value | Conditions (resolution, format, etc.) |
| -------------------- | ----- | ------------------------------------- |
| FPS                  | TODO  | TODO                                  |
| Latency              | TODO  | TODO                                  |

**Sample frames:** TODO — add captured images here.

## Roadmap

- **m1 — csi-inspector:** implement `csi_inspect.c` and the `Makefile` (in progress).
- **TODO:** Subsequent modules (m2, m3, …) have not been defined in the repository yet.

## License

No license file is present in this repository yet. **TODO:** choose and add a `LICENSE` file.
Until then, all rights are reserved by the author.
