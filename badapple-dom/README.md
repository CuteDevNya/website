# Bad Apple // DOM Visualizer

A static, dependency-free GitHub Pages experiment that renders each video frame as a field of randomly styled HTML elements.

## Open the website

https://robloxprogrammer00.github.io/website/badapple-dom/

## Add your video

1. Put your own video file in this folder and name it `bad-apple.mp4`.
2. Commit and push it to GitHub. The deployed page will load it automatically.
3. Alternatively, open the page and use **Video wählen** to load a local `.mp4`, `.webm` or `.ogv` file without uploading it anywhere.

The video is intentionally not included in this repository. That keeps the repository small and lets you choose your own copy.

## Controls

- **Play / pause:** playback with the video's audio.
- **Restart:** start again from the beginning.
- **Resolution:** set how many HTML elements are used to represent a frame.
- **Invert brightness:** reverse the mask if your copy has a different black/white polarity.
- **Black threshold:** leave more dark areas empty or bring out darker details.
- **Fullscreen:** expand the visualizer.

## How it works

The browser draws each video frame to a tiny off-screen canvas, samples the luminance of each grid cell and changes the opacity of its corresponding DOM element. Each element gets a randomized shape, color, size and rotation. There are no external libraries and no server-side processing.

Only use video and audio files you have the right to use.
