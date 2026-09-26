# RigLogic 0.12.4 — First Public Release

RigLogic is a control-translation layer for Windows and Linux. It sits between physical controller hardware and the game, letting you clean up, reshape, translate, and monitor inputs without replacing the rest of your rig.

## Highlights

- Analog calibration, deadzones, inversion, response curves, smoothing, and lower-deadzone tuning.
- Digital modes for holds, taps, transitions, paired commands, toggles, thresholds, and prerequisites.
- Fast encoder and short-event handling designed not to lose quick clicks.
- Multi-position selector conversion to virtual buttons or relative adjustment commands.
- Stable virtual assignments so adding a mapping does not shuffle existing in-game bindings.
- Signal Labs recording for real driving sessions with synchronized raw, calibrated, filtered, and accepted/submitted traces.
- Offline comparison of proposed filters and timing without sending test output to the game.
- Independent pinned overlays plus the embedded selected-mapping preview.
- Portable profiles that remember separate Windows and Linux hardware connections.
- Guided Linux input-access setup and removal, including automatic setup when Start outputs needs uinput access.

## Platforms

Windows x64 and Linux x64 are included. Windows virtual-controller output uses a compatible x64 vJoy installation. Linux uses evdev for physical input and uinput for generated output.

Linux supports X11 and native Wayland. KDE/wlroots floating overlays use the bundled layer-shell runtime. GNOME Wayland uses the optional RigLogic Input Monitors companion.

## Safety

RigLogic is not an emergency stop and does not replace independent motion-rig safety hardware. Verify every mapping in the intended game before driving.
