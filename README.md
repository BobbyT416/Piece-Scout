# Piece Scout v2.0

Piece Scout is a browser prototype for finding where physical jigsaw pieces belong.

## What changed in v2.0

This is the first real computer-vision milestone. The app now:

1. Loads a completed puzzle/reference photo.
2. Loads a photo of loose pieces.
3. Uses OpenCV.js in the browser to estimate the table/background color and detect separated piece contours.
4. Uses ORB feature matching plus a RANSAC homography to estimate where each detected piece appears in the reference image.
5. Places touch/click targets over detected pieces.
6. Shows a red predicted location on the completed puzzle when a piece is selected.

The sample test remains available and keeps its known mapping so the interface can be tested independently of computer vision.

## Important limitations

This is an early CV engine, not a finished puzzle solver. It works best with:

- a mostly straight-on reference image;
- a clear completed-puzzle image rather than a heavily angled box photo;
- loose pieces separated from each other;
- a plain, reasonably uniform table/background;
- good lighting and limited glare;
- puzzle artwork with enough visual detail for feature matching.

The next engineering milestones are better piece segmentation, perspective correction, edge/shape analysis, stronger artwork matching for low-texture pieces, rotation estimation, neighboring-piece suggestions, and support for large piece counts.

## GitHub Pages

Upload the contents of this folder to a repository and enable GitHub Pages for the branch/folder containing `index.html`.

OpenCV.js is loaded from the official OpenCV documentation CDN, so the deployed page needs internet access for the CV library.
