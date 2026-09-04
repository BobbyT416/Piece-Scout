# Piece Scout v2.7.1

GitHub Pages-ready prototype for Piece Scout.

## v2.7.1 changes
- Clean startup; no automatic puzzle load.
- Larger phone/tablet photo buttons.
- Faster mobile analysis: reference features are computed once instead of once per piece.
- Caps working image dimensions during feature extraction to reduce browser memory/CPU pressure.
- Incremental progress updates while pieces are matched.
- Aurora 12 benchmark and sample test remain available.
- Visible version number in the footer.

## Test
1. Open the app.
2. Choose **Load Aurora 12 benchmark**.
3. Choose **Analyze puzzle**.
4. Watch the progress message while it processes each piece.

This is still an experimental computer-vision prototype.
