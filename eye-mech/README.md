# EyeMech ε3.2 — Will Cogley

These are Will Cogley's eye mechanism files: 3D prints, the assembly guide, the controller board and the control code. They're copied here so the whole project is in one place.

**Designed by [Will Cogley](https://www.willcogley.com).** Eyeballs and the official controller board are sold at [nmrobots.com](https://nmrobots.com/).

## License

This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/):

- **BY:** credit Will Cogley.
- **NC:** non-commercial use only. For commercial use, contact enquiries@willcogley.com.
- **SA:** anything you share that's built from these files must use the same license.

The controller board is based on the open-source MAIGIFU board by [@suzan_works](https://oshwlab.com/suzan_works/rp2040_pico-compatible_maigifu_2).

The rest of this repository (the simulator and the AI code) is our own work. The license above applies only to the files in this `eye-mech/` folder.

## What's here

| Folder | Contents |
| --- | --- |
| `EyeMech_3.2_Assembly_Document.pdf` | The parts list, print settings, assembly, wiring and calibration guide. **Start here.** |
| `print/EyeMech_3.2_Testing_Plate.3mf` | Servo sizing plate. Print it first to pick variant A or B. |
| `print/EyeMech_3.2_MG90s_-_A.3mf` / `-_B.3mf` | The full mechanism for MG90S servos (our choice). |
| `print/EyeMech_3.2_SG90_-_A.3mf` / `-_B.3mf` | The full mechanism for SG90 servos. |
| `print/EyeMech_3.2_All_Plates*.3mf` | Every part on pre-made plates. The `BambuStudio` version is for Bambu printers. |
| `print/EyeMech_e4.0_Changed_4_Lids_and_2_Central_bars.3mf` | A modified version that includes a `CameraEye` part. Saved for the camera step later. |
| `board/` | Controller board: Gerber files, BOM, pick-and-place file and schematic (v1.3). These are the files to order it assembled from JLCPCB. |
| `code/EyeMechEpsilon3.py` | Will's original MicroPython control code. Save it to the board as `main.py`. |

## Quick start

1. Print the Testing Plate, test-fit an MG90S, and note whether hole A or B fits best.
2. Print the matching `MG90s` file (PLA, 0.2 mm layers, tree supports).
3. Assemble, flash, and calibrate by following the assembly PDF.
