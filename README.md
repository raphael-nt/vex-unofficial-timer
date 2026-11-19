# VEX Unofficial Timer

A 60 second match timer in the browser for VEX GO practice.

Live page : https://irap.club/vex-unofficial-timer/

This is an unofficial practice tool. It is not affiliated with or endorsed by VEX Robotics.

## Credit

The look of the timer and every sound in `sounds/timer.mp3` come from the video "UPDATED VEX IQ Official Timer with 3 sec countdown" by Ben Lipper : https://www.youtube.com/watch?v=ZEBHVsnhAi4

## Modes

- **Teamwork Challenge** : 3, 2, 1 countdown, then 60 seconds of driver control. From 0:35 to 0:25 the bar shows DRIVER SWITCH and the controller icon blinks. A sound plays and the time flashes orange at 0:35 and 0:25.
- **Robot Skills Challenge** : 3, 2, 1 countdown, then 60 seconds of driver control with no switch window.

In both modes the last 10 seconds are shown in yellow and the end sound plays at 0:00. The 3, 2, 1 countdown plays the beeps and the start sound as one piece, with the numbers timed to the beeps like the reference video.

## Keys

| Key | Action |
|---|---|
| Space | Start, pause and resume |
| Left / Right arrow | Move the match time back or forward 1 second |
| Tab | Switch between Teamwork and Robot Skills (only when no match is running) |

Every key can be changed in the settings. Keys use `KeyboardEvent.code`, so they work with any keyboard layout.

## Seek bar

- Moving the mouse or touching the screen during a match shows the blue seek bar. It fades out with the corner buttons after 2.5 seconds without movement.
- Pausing shows the seek bar and keeps it on screen until the match resumes, then it hides at once.
- The right end shows the time like YouTube, for example 0:25 / 1:00 (time played out of the full match).
- Seeking with the arrow keys shows the bar, which fades out after the key is released.
- Click or drag on the bar to jump to a time. White marks show 0:35 and 0:25 in Teamwork mode.
- Seeking does not play the 0:35, 0:25 or end sounds. They only play when the clock runs past them.

## Settings

The gear in the bottom left holds every setting : mode, volume, keys, and a link to VEX GO Builder. The page is in English only. Settings are kept in the browser with localStorage.

Play and reset buttons sit in the bottom right corner and the full screen button in the top right corner. They hide while a match runs and come back when you move the mouse or touch the screen.

Sizes follow the screen (vw, vh and vmin units), from phones to 4K projectors.

## Files

- `index.html` : the whole app in one file, no build step and no external libraries.
- `sounds/timer.mp3` : audio of the reference video. The page plays short parts of it with the Web Audio API. If the file cannot load, generated tones are used instead.

Hosted with GitHub Pages from the `main` branch root.
