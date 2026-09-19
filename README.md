# XPadCheck360

A real-time controller diagnostic suite and analog stick drift-testing utility built natively for modified Xbox 360 consoles (**RGH / JTAG / Devkit**).

Designed to provide pinpoint hardware diagnostics, **XPadCheck360** gives you an instant, raw-data view of your gamepad's internal sensors, deadzones, and wireless connection health.

---

## 🎮 Features & Diagnostics

* **Thumbstick Drift & Axis Scope**  
  Visualizes resting position and live stick travel on twin radar scopes. Displays raw input integers (`-32,768` to `32,767`), real-time deflection percentages, and Euclidean drift magnitude. Includes official Microsoft factory circular deadzone rings (**7,849** for Left Stick, **8,689** for Right Stick) to easily spot physical drift, loose centering springs, or worn potentiometers.

* **Analog Trigger Tracking**  
  Measures left and right analog trigger travel from `0` (unpressed) to `255` (fully depressed) with color-coded gauge bars to detect dead travel or sensor wear.

* **Digital Input Matrix**  
  Complete visual mapping for all digital inputs: face buttons (**A**, **B**, **X**, **Y**), D-pad directions, bumpers (**LB**, **RB**), and thumbstick clicks (**LS**, **RS**), featuring active color-shift indicators upon press.

* **Rumble Motor Testing**  
  Dedicated vibration testing routine driving the low-frequency heavy weight (held via **LB**) and high-frequency light weight (held via **RB**) at full power to verify motor functionality.

* **Wireless Packet & Link Diagnostics**  
  Tracks incoming XInput packet sequence numbers (`dwPacketNumber`) in real time to diagnose wireless sync issues, signal drops, or high-latency RF environments.

* **4-Port Controller Scanner**  
  Simultaneously monitors console hardware ports **P1** through **P4** to verify controller detection and slot assignments without needing to reboot the dashboard.

---

## 📥 Installation & Updates

Choose either of the two installation methods below:

### Option 1: Automatic Over-the-Air Update (Recommended)

Keep `updater.xex` in the same directory as `default.xex` on your console's hard drive or USB drive.

1. Launch **`updater.xex`** via Aurora or XeXMenu.
2. Press **[A] Check Updates** to query GitHub for the latest release.
3. If a new version is detected, select **[A] Download** — the updater will stream the binary directly over the network and replace `default.xex` in place without needing a PC.

---

### Option 2: Manual Installation

1. Go to the **[Releases](https://github.com/Retrozcube/XPadCheck360/releases)** page on this repository.
2. Download the latest pre-compiled **`default.xex`** binary.
3. Copy the file into your console folder (e.g., `Hdd1:\Apps\XPadCheck360\`) via USB or FTP, replacing your existing executable.
