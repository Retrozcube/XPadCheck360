XPadCheck360
A real-time controller diagnostic suite and analog stick drift-testing utility built natively for modified Xbox 360 consoles (RGH / JTAG / Devkit).

Designed to provide pinpoint hardware diagnostics, XPadCheck360 gives you an instant, raw-data view of your gamepad's internal sensors, deadzones, and wireless connection health.

What It Does
Thumbstick Drift & Axis Scope: Visualizes analog stick resting position and deflection on twin radar scopes. Displays raw input integers (-32,768 to 32,767), real-time deflection percentages, and live Euclidean drift magnitude calculation. Includes official Microsoft factory circular deadzone rings (7,849 for Left Stick; 8,689 for Right Stick) so you can immediately spot physical stick drift, loose centering springs, or worn potentiometers.

Analog Trigger Tracking: Measures left and right analog trigger travel from 0 (unpressed) to 255 (fully depressed) with color-coded gauge bars to identify dead travel or sensor degradation.

Digital Input Matrix: Full visual mapping for face buttons, directional pad, bumpers, and thumbstick clicks (LS / RS), featuring active color-shift indicators upon press.

Rumble Motor Testing: Dedicated vibration test routine driving the low-frequency heavy weight (held via LB) and high-frequency light weight (held via RB) at full power to verify motor functionality.

Wireless Packet & Link Diagnostics: Tracks incoming XInput packet sequence numbers (dwPacketNumber) in real time to diagnose wireless sync issues, signal drops, or high-latency RF environments.

4-Port Controller Scanner: Simultaneously scans console hardware ports P1 through P4, allowing quick identification of connected controllers without needing to reboot the dashboard.

How to Install & Update
You can keep XPadCheck360 up to date using either of two methods:

Option 1: Automatic Over-the-Air Update (Recommended)
Keep updater.xex in the same directory as default.xex on your console's hard drive or USB drive:

Launch updater.xex via Aurora or XeXMenu.

Press [A] Check Updates to query GitHub for the latest release.

If a new version is detected, select [A] Download — the updater will stream the binary directly over the network and overwrite default.xex in place without needing a PC.

Option 2: Manual Installation
Navigate to the Releases page on this repository.

Download the latest pre-compiled default.xex asset.

Transfer the file to your console folder (e.g., Hdd1:\Apps\XPadCheck360\) via USB or FTP, replacing your existing executable.
