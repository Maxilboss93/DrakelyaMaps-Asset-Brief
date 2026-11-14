# Varied western ridge study v4

Experimental, not enabled in the editor or provider catalog. The massif is the
unchanged v3 source; the new saddle is generated with the built-in image tool
using that source as the sole style reference. Both originals are retained.
Stable STUDY IDs must not be saved in real worlds.

Prompt direction: exactly the reference's delicate ink/watercolor and sand-gold,
grey-olive palette, but a lower asymmetrical two-summit saddle and curved folded
shoulder; narrow broken base, upper-left light, no apron, halo, scenery, buildings,
snow, labels or frame. True transparent background. Not a rotated or stretched
copy of the tall massif. Alpha crop/WebP preparation is the existing script with
STUDY_KIT_VERSION=4, accepting massif then saddle source PNGs.

## Fixed-region test

STUDY_MANUAL_KIT=4 uses six alternating high/low groups in the existing reference
harness. Low footprints have closer baselines so the saddle does not introduce a
new gap. No source terrain, towns or roads were changed. The comparison image is
manual-kit-v4-comparison.png in the reference-region output directory.

Assessment: varied silhouettes reduce the uniform high-peak repetition; the
towns remain readable. The narrow chain is still visibly assembled, and the
lighter new section does not fully match neighboring older art. This is an
incremental improvement, NOT an accepted match to the reference or permission to
activate automated generation. Bounding-box overlap does not prove connected
opaque silhouettes; actual renderer screenshots remain the visual gate.

Eight focused tests passed: file hashes/runtime exclusion, native proportions,
immutable geography, fixed settlement clearances, alternating IDs, overlap and
unchanged instance count. Real editor desktop/mobile rendering passed with no
JS/shader errors and a nonblank canvas. Full regression/build not repeated for
this isolated source-art and test-harness change. Cloud/export not tested.

Scene: 368 art instances, 28 textures, 15,171,968 decoded bytes. Versus v3 connected:
same instance count, one extra texture and 374,784 additional decoded bytes.
New compressed saddle: 77,470 bytes. Single-run terrain worker time 4,884.4 ms;
do not infer a performance improvement from timings across separate runs.

## Interactive local review

Set STUDY_SOURCE to the fixed 384x288 reference document and run
`node tests/manual-study-preview.mjs`. Open `http://localhost:3299/__study/`.
This test harness uses the actual editor, with isolated Vite transforms for the
experimental art and terrain. It does not change the production renderer.
Study materials receive a subtle RGB tint (0.92, 0.94, 0.96); source images remain
unchanged. API calls are blocked and no saved cloud world is modified.

Use this preview to inspect, pan and zoom the western chain. The six placements
are fixed to this reference region, not an automatic composer: do not resize or
regenerate the document as a test of general generation. Local export does not
serialize the experimental derived artwork. Local storage belongs to the
separate preview origin, not the normal editor on port 3202.

`tests/manual-study-preview.browser.mjs` checks the real canvas, sheet zoom,
desktop/mobile rendering, blocked backend and JavaScript errors. Mobile after
zoom retains that zoom and requires panning; this is not a mobile UX approval.
Eight asset/composition tests also pass. Full build and cloud save/reopen were
not repeated for this test-only preview.
