# Public Development review bundle — immiscible_u_tube_equal_density_pressure_error

Static public mirror of the Development review page for the counterfactual generator
`immiscible_u_tube_equal_density_pressure_error`.

- Source PR: https://github.com/hipo-dev/counterfactual-data/pull/739
- Exact source head: `41b763582970b581753ecac790648582f18d9c0a`
- Evidence identity: `eb9ee584295ced3bc885a36f0c90073ff6db959b554dd480a5b4cba0f4289f97`
- Authoritative review origin: https://13-216-208-230.sslip.io/demos/2026-10-19_two-liquid-u-tube-41b7635/

## What is in this bundle

- `index.html` — the Development review page: three cases, each with four synchronised
  players (True, Counterfactual, Binary Mask, Mask Overlay), complete standalone prompts,
  mechanism and viewing cues, and collapsed complete metadata.
- Per case: `true/video.mp4` and `counterfactual_equal_density_pressure/video.mp4`
  (native 2048x2048, 24 fps, 120 frames, H.264),
  `counterfactual_equal_density_pressure/mask.mp4` (strict binary mask, black/white
  `{0,255}`, three equal RGB channels) and
  `counterfactual_equal_density_pressure/mask_overlay.mp4` (client-facing review overlay:
  active mask pixels are pure red `#FF0000`, pixels outside the mask keep the
  Counterfactual RGB unchanged). The `web/` folders hold 1024x1024 browser viewing copies.
- Audit attachments: `decoded-audit.json`, `scale-audit.json`, `review-summary.json`,
  `runtime-witness.json`, `runtime-witness-index.json`, `runtime-provenance-audit.json`,
  `review-manifest.json`, `html-workflow-evidence.json`, `final-evidence-seal.json`.

The formal binary mask contract and the client-facing red overlay are separate artefacts.
All review bundle files are byte-identical to the published EC2 bundle; the EC2 origin
remains the authoritative copy and this mirror exists so the page stays reachable even when
the shared worker is stopped.

Human acceptance of this exact head is still pending; this bundle does not assert Gate B/C
approval, a Full run or a merge.
