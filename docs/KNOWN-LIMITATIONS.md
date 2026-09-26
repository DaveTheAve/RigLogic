# Known Limitations — RigLogic 0.12.4

RigLogic 0.12.4 is the first public pre-1.0 release. These are current platform limits rather than hidden failures.

## Windows

- Virtual-controller output requires an existing compatible x64 vJoy installation. Keyboard-only mappings do not require vJoy.
- The public build is portable rather than installer-based.
- Unsigned builds may trigger Windows SmartScreen or show an Unknown Publisher warning until code signing is added.

## Linux

- The first use of virtual output requires one authorized udev-rule setup for joystick input and /dev/uinput. RigLogic can remove that exact rule later from Settings.
- Native Wayland support depends on the compositor and working EGL support. Avalonia's native Wayland backend remains experimental upstream.
- KDE Plasma and wlroots compositors can use native layer-shell floating overlays. GNOME Wayland requires the optional per-user companion for floating overlays.
- A new GNOME Shell companion installation may require signing out and back in before it can be enabled.
- The public Linux build targets x64 glibc systems. Other architectures are not part of this release.

## Games and hardware

- RigLogic cannot read a game's current value for relative selector commands; those commands require an explicit or assumed reference.
- Physical controllers remain visible to the operating system. Clear duplicate raw bindings in the game when binding the RigLogic virtual output.
- A handbrake connected through a wheelbase should not cause the entire wheelbase to be hidden or grabbed; steering and force feedback still need their native connection.
- Anti-cheat, driver policy, and game input behavior vary by title. RigLogic does not bypass platform or game security controls.

## Pre-1.0

Profiles and virtual assignments are designed to remain stable, but pre-1.0 releases may still change UI, diagnostics, and unsupported edge cases. Back up profiles and rig-registry.json together before major updates.
