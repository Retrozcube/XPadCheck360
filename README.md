# XPadCheck360

A dedicated, lightweight controller diagnostic and analog stick drift testing utility for modified Xbox 360 consoles (RGH/JTAG).

Built with raw Direct3D 9 and XInput, XPadCheck360 provides real-time telemetry, button response monitoring, and calibrated deadzone testing to inspect and diagnose OEM and aftermarket Xbox 360 gamepads.

---

## Features

* **Precision Stick Drift Scope:** Live Euclidean radial deadzone visualization using official Microsoft SDK thresholds (LS: `7849`, RS: `8689`).
* **Real-Time Axis Telemetry:** Displays raw integer values (`-32768` to `32767`), deflection percentages, and total drift magnitude vectors.
* **Analog Trigger Gauges:** 8-bit precision bars (`0` to `255`) for inspecting potentiometer sweep and trigger wear.
* **Full Digital Button Mapping:** Visual state tracking for face buttons, D-pad directions, shoulder bumpers, and thumbstick clicks.
* **Rumble Motor Testing:** Dedicated trigger tests for both heavy (left) and light (right) vibration motors.
* **Overscan Safe Layout:** Engineered within title-safe display margins for full visibility on standard CRT and modern HDTV displays.

---

## Installation

1. Download the latest `default.xex` from the [Releases](https://github.com/Retrozcube/XPadCheck360/releases) tab.
2. Copy `default.xex` to your console storage (e.g., `Hdd1:\Apps\XPadCheck360\default.xex`) via USB or FTP.
3. Launch the application using Aurora, DashLaunch, Freestyle Dash, or XeXMenu.

---

## Controls

| Input | Action |
| :--- | :--- |
| **Left Stick / Right Stick** | Real-time position & drift scope testing |
| **LT / RT** | Analog trigger actuation sweep (`0–255`) |
| **LB (Hold)** | Test heavy vibration motor |
| **RB (Hold)** | Test light vibration motor |
| **Face Buttons / D-Pad** | Digital switch responsiveness check |

---

## Building from Source

* **IDE:** Microsoft Visual Studio 2010
* **SDK:** Xbox 360 SDK (XDK)
* **Post-Processing:** Use `xextool` to package the compiled `.xex` binary for retail/RGH execution:
  ```cmd
  xextool.exe -m r -r a -e u -o default.xex XPadCheck360.xex
