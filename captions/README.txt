Source photo captions
=====================

Start with index.jsonl for text-only review. It has one JSON object per source
file, with the full caption and project-relative image and sidecar paths.
Sidecars under sidecars/ contain the same descriptions as single lines of UTF-8
text. They cover visible clothing, pose, framing, and scene details.

Reading the index
-----------------

- Width, height, and orientation describe the image as displayed with EXIF
  rotation applied. Visible black bands also receive a black_bars observation.
- Framing describes the visible extent of the subject. three_quarter means a
  crop near the thighs or knees. face_cropped identifies torso-centered photos
  where the camera frame cuts through the face.
- Face view describes head direction relative to the camera. Face visibility
  identifies clear, small, partial, blocked, cropped, and rear-view faces.
  These are approximate visual descriptions. small indicates scale in the
  source image and carries no training threshold.
- Expression is a visible mouth or smile cue. closed_lips includes neutral,
  pursed, and slight closed-mouth smiles. smile leaves tooth visibility open.
  unclear means the captioner could not confidently tell.
- Setting groups indicate shared visual context. Use them as leads when
  investigating capture sessions. exact_duplicate_of points to the original-
  named copy in each byte-identical pair, verified by SHA-256. Similar but
  byte-different photos still need a separate comparison during the audit.
- The clothing_coverage_unclear observation on source/IMG_4387.JPG records an
  ambiguous bedroom mirror photo. Ask the creator or a human reviewer to check
  the original and confirm what is visible before including it in a visual
  agent task. Its neutral caption remains available for text-only indexing.

FluxGym handoff
---------------

FluxGym matches uploaded .txt files to images by basename. When a training
subset and trigger are decided, pair each selected source photo with a working
copy of its matching sidecar. Add the agreed trigger to those working captions
and check the imported text in FluxGym. The current sidecars contain only the
descriptive caption. Upstream documentation and import code are at
https://github.com/cocktailpeanut/fluxgym#uploading-caption-files and
https://github.com/cocktailpeanut/fluxgym/blob/main/app.py.

Training usefulness, inclusion decisions, and the final caption strategy
belong to the later research-backed audit.
