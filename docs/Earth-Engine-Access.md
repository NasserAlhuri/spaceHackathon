# Earth Engine execution and reference access — 8 October 2026

Nasser completed authorized Code Editor setup, corrected the masked-fallback runtime error, ran the September 2021/2026 workflow and exported eight files on 7 October. The supplied [external export review](Dynamic-World-External-Export-Review.md) records that successful execution history. A stale hard-coded local failure message was not evidence of Code Editor failure. Do not ask Nasser to repeat account setup or send secrets in chat.

All eight exact original files are now locally verified: the five CSVs and transition TIFF were received through Drive; the two annual TIFFs were reconstructed from six uploaded parts on 8 October. Every part and both output hashes match REASSEMBLY.json and the already recorded export identities. Complete actual raster checks passed. The earlier 32 MiB transfer problem has been resolved by parts. The original external ZIP's archive hash was not independently checked. See [current technical/scientific report](Dynamic-World-Reassembly-and-Scientific-Review.md).

The previous managed-runtime EE/Earth Search requests returned CONNECT 403 under the configured proxy, with no Google identity/project bindings. This runtime has not independently fetched those assets or bypassed network/TLS policy. Nasser has now supplied the corresponding 1/26 September 2021 reference RGB/QA60 exports and original source CSV. The reference-availability blocker is resolved through these actual files, separately from direct API access. No repeat export or account setup is needed.

All three unique supplied files match recorded SHA256; the 20210901(1).tif duplicate was byte-identical and ignored. Source IDs/acquisition timestamps match the original DW provenance locally. Both four-band UInt16 TIFFs have the exact study grid. All 18 target/context pixels are valid, with QA60=0 and declared scene cloud 0%; these are screening facts, not perfect cloud/visibility truth. The preliminary review covered all 72 views across four dates. [Actual paired observations and limits](Dynamic-World-Paired-Reference-Review.md) distinguish eight clear broad patterns, ten exact-class ambiguities and three overlapping potential disagreement flags. Independent scientific and teammate reviews remain pending.

The unchanged plan uses the same analyst-defined rectangle, September 1 inclusive to October 1 exclusive, fixed EPSG:32639 10 m grid, mean probabilities, minimum 3 observations and confidence 0.60 with 0.50/0.70 sensitivity. The 50% common-window gate remains failed at primary 30.9385%. No general historical-change result is adopted. 2023, SamGeo and other models remain deferred.

Reproduce read-only checks in a scientific environment with numpy/rasterio/pyproj:

```bash
python src/validate_dynamic_world_references.py
python src/render_dynamic_world_paired_review.py
python src/validate_dynamic_world.py --exports data/dynamic_world/raw/2026-10-07 --output results/dynamic-world-table-verification.json
python src/validate_dynamic_world_rasters.py --exports data/dynamic_world/raw/2026-10-07 --manifest metadata/dynamic-world-export-manifest.json --output results/dynamic-world-raster-verification.json
```

Original source identifiers remain unchanged; canonical paths derived from declared dataset/index remain explicitly not independently fetched. The saved future export mask/provenance correction has not generated new server exports. Reading the original exports, complete numeric/raster integrity, reassembly and completed 18-location/72-view paired preliminary review do not establish independent exact-class accuracy or citywide change. Independent scientific/member acceptance remains pending. No submission or organizer contact is authorized or performed.

The [7 October access record](history/Earth-Engine-Access-2026-10-07.md) is preserved with its then-incomplete transfer status; it is superseded by this checkpoint.
