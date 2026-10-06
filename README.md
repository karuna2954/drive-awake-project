# DRIVE AWAKE — Driver Monitoring System

A standalone frontend prototype for AI-based driver drowsiness and distraction detection.

## Run

No npm or build step is required.

1. Open `index.html` in a modern browser.
2. Use **Launch Safety Monitor**.
3. Use **START SIMULATION** to demonstrate drowsiness/distraction events.
4. Use **Enable Camera** to preview the browser camera. The current frontend deliberately labels the camera metrics as simulated; it does not claim that a real AI model is running.

For camera permissions, a local server is more reliable than opening the file directly. From this folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## What is included

- Automotive-style dark dashboard
- Overview and product hero
- Live driver monitor
- Simulated face/landmark overlay
- Drowsiness metrics: EAR, PERCLOS, yawning, head movement
- Distraction metrics: gaze, head pose, phone/object evidence
- AI/CNN architecture visualization
- Risk engine and alert levels
- Event timeline and filtering
- Performance charts
- Testing scenarios
- Privacy controls
- Hardware/software deployment roadmap
- Browser camera permission flow
- Scripted drowsiness + distraction demo simulation

## Important

This is a **web UI prototype**, not a validated safety-critical AI system. The live camera view currently does not run MediaPipe/OpenCV/CNN inference in the browser. To make the project a real AI system, connect an actual face-landmark/model inference pipeline and replace the simulated telemetry with model outputs.
