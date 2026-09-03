# Piece Scout

First GitHub Pages prototype for Piece Scout.

## What this build does

- Loads a completed-puzzle image and a loose-pieces image.
- Provides the planned Piece Scout workflow.
- Includes a sample 80-piece test mode.
- In sample mode, tapping a piece highlights its location in the completed puzzle and shows possible neighboring pieces.
- Runs as a static site; no server is required.

## GitHub Pages

Upload `index.html`, `sample_reference.png`, and `sample_pieces.png` to the repository root.

Then enable:

**Settings → Pages → Deploy from a branch → main → / (root)**

## Important

The sample interaction uses a known test mapping. Arbitrary user photos are intentionally not given fake matches yet. The next milestone is the actual computer-vision engine that detects pieces, identifies their artwork/shape, and matches them to the reference puzzle.
