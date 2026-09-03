# Piece Scout v2.2

GitHub Pages prototype for the Piece Scout puzzle-piece locator.

## What's new in v2.2
- Adds a **Load Aurora 12 benchmark** button.
- The benchmark downloads a known matched pair from the public `Devanshusp/jigsaw-puzzle-solver` dataset:
  - `aurora.png` = completed/reference image
  - `aurora12.png` = same puzzle represented as 12 scrambled pieces
- Uses the existing browser-side OpenCV pipeline for segmentation, SIFT/ORB feature matching, rotation testing, and RANSAC verification.
- Keeps the known-good 80-piece interface sample.
- Visible version number: **Piece Scout v2.2**.

## Test order
1. Open the page.
2. Wait for OpenCV to finish loading.
3. Click **Load Aurora 12 benchmark**.
4. Click **Analyze puzzle**.
5. Report how many pieces are detected and how many are matched.

The benchmark source is the public GitHub project documented here: https://github.com/Devanshusp/jigsaw-puzzle-solver

## Important
This remains an experimental computer-vision prototype. The Aurora benchmark image is a controlled dataset image, not a photograph from a phone camera. Real-world photos will require additional perspective correction, segmentation, and matching improvements.
