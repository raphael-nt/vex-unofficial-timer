# VEX Unofficial Timer

A 60 second match timer in the browser for VEX GO practice.

Live page : https://irap.club/vex-unofficial-timer/

This is an unofficial practice tool. It is not affiliated with or endorsed by VEX Robotics.

## Modes

- **Teamwork Challenge** : 3, 2, 1 countdown, then 60 seconds of driver control. From 0:35 to 0:25 the bar shows DRIVER SWITCH and the controller icon blinks. A sound plays and the time flashes orange at 0:35 and 0:25.
- **Robot Skills Challenge** : 3, 2, 1 countdown, then 60 seconds of driver control with no switch window.

In both modes the last 10 seconds are shown in yellow and a buzzer plays at 0:00.

## Use

- Play and reset buttons sit in the bottom right corner. They hide while a match runs and come back when you move the mouse or touch the screen.
- The gear in the bottom left holds every setting : mode, language (Thai or English), sound, full screen, and a link to VEX GO Builder.
- Settings are kept in the browser with localStorage.
- Sounds are generated with the Web Audio API, so there are no audio files.

## Files

- `index.html` : the whole app in one file, no build step and no external libraries.

Hosted with GitHub Pages from the `main` branch root.
