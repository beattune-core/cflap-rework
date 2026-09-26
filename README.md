# cflap-rework

An open-source air divider ("flap") for CPAP-based part cooling on 3D printer toolheads. A flap inside the divider, driven by a servo or a stepper, routes the air from a single CPAP blower between outlets.

> **Status: early release.** This first release contains the STL files for the **servo version** only. The stepper version, the source CAD files and the printer macros will follow in later releases.

<!-- TODO: add a photo or render of the assembled divider -->
<!-- ![cflap-rework assembled](docs/images/assembly.jpg) -->

## Repository layout

```
stl/
├── servo/                  # Servo-driven divider
│   ├── mainbody.stl
│   ├── flap.stl
│   ├── top_cover.stl
│   ├── top_cover_tpu_seal.stl
│   ├── bottom_plate.stl
│   └── bottom_plate_tpu_seal.stl
└── air hose adapter/       # Hose adapters for the Mellow CPAP
    ├── Mellow_cpap_hose_intake.stl
    └── Mellow_cpap_hose_exhaust_2x.stl
cad/                        # Source CAD files (coming later)
```

## Parts to print

### Servo version (`stl/servo/`)

| Part                        | Qty | Material        | Notes                          |
| --------------------------- | --- | --------------- | ------------------------------ |
| `mainbody.stl`              | 1   | ABS / ASA       |                                |
| `flap.stl`                  | 1   | ABS / ASA       |                                |
| `top_cover.stl`             | 1   | ABS / ASA       |                                |
| `bottom_plate.stl`          | 1   | ABS / ASA       |                                |
| `top_cover_tpu_seal.stl`    | 1   | TPU             | Seals the top cover            |
| `bottom_plate_tpu_seal.stl` | 1   | TPU             | Seals the bottom plate         |

### Hose adapters (`stl/air hose adapter/`)

| Part                              | Qty | Material  | Notes                                   |
| --------------------------------- | --- | --------- | --------------------------------------- |
| `Mellow_cpap_hose_intake.stl`     | 1   | ABS / ASA | Connects the CPAP hose to the divider   |
| `Mellow_cpap_hose_exhaust_2x.stl` | 1   | ABS / ASA | File contains two exhaust adapters      |

<!-- TODO: confirm materials and add recommended print settings (layer height, walls, infill, supports) -->

## Bill of materials

<!-- TODO: fill in the exact hardware -->

| Item                 | Qty | Notes                          |
| -------------------- | --- | ------------------------------ |
| Servo                | 1   | Model: MG90S                   |
| Screws               | _TBD_ | Size and length: _TBD_       |
| Heat-set inserts     | _TBD_ | Size: _TBD_ (if used)        |

## Assembly

<!-- TODO: add step-by-step assembly instructions with pictures -->

1. Print all parts listed above.
2. Place the flap in the main body.
3. Fit the TPU seals to the top cover and the bottom plate.
4. Mount the servo and connect it to the flap.
5. Close the main body with the top cover and the bottom plate.
6. Attach the intake and exhaust hose adapters and connect the CPAP hoses.

## Firmware and macros

Printer macros for controlling the flap will be published in a later release.

## Roadmap

- [x] STL files for the servo version
- [ ] STL files for the stepper version
- [ ] Printer macros
- [ ] Source CAD files
- [ ] Assembly guide with pictures

## Contributing

Issues and pull requests are welcome. If you build one, photos and feedback on fit, sealing and airflow help improve the design.

## License

<!-- TODO: choose a license, e.g. CERN-OHL-S-2.0 or CC BY-SA 4.0 for hardware, and add a LICENSE file -->
_License to be added._
