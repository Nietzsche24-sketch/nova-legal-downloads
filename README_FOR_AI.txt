# NovaLegal Atlas — Tachyon Anchor

Court-ready and searchable Ontario Application Record bundles (Atlas-grade).
One-click release pipeline, conservative validation, GitHub-hosted artifacts.

## Current Release
- Tag: `v2025.09.07-app3`
- Title: *Smith v Ontario — Application Record*
- Artifacts: `smith_full_bundle.zip`, `smith_review.zip`, `SHA256SUMS.txt`

## One-Click Release
Run this from the folder with your _deliverables:
nova_release "Smith v Ontario — Application Record" appX ~/Desktop/atlas_test/_deliverables

## Verify a release from GitHub
TAG=v2025.09.07-app3
BASE="https://github.com/Nietzsche24-sketch/nova-legal-downloads/releases/download/$TAG"

mkdir -p ~/tmp/release-check && cd ~/tmp/release-check
curl -LO "$BASE/smith_full_bundle.zip"
curl -LO "$BASE/smith_review.zip"
curl -LO "$BASE/SHA256SUMS.txt"

# Keep only the Smith zip rows, normalize spacing to "SHA  filename"
grep 'smith_.*\.zip' SHA256SUMS.txt > SHA256SUMS.smith.txt
awk '{print $1"  "$2}' SHA256SUMS.smith.txt > SHA256SUMS.fixed

# Check
shasum -a 256 -c SHA256SUMS.fixed

## Gotchas
- Harmless qpdf warnings like “unexpected EOF” can appear.
- Prefer `qpdf --linearize` before zipping.
- Ghostscript pstopdf shim is in place.
- Deliverables always include [court + searchable + README].
