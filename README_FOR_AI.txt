# Tachyon Anchor

This file helps us (AI + Peter) remember the release process.

- Repo: nova-legal-downloads
- Last release: Smith v Ontario — Application Record
- Workflow: nova_release → upload → verify checksums → push → publish
- Checkpoint date: Sun  7 Sep 2025 04:01:41 EDT


## Release Summary (Smith v Ontario — Application Record)

- **Tag**: v2025.09.07-app3  
- **Bundles**:
  - smith_full_bundle.zip — Court bundle + Searchable bundle + README  
  - smith_review.zip — Searchable-only + README  
- **Checksums**:
  - SHA256SUMS.txt uploaded with both ZIPs  
- **Verification**:
  - Both zips passed checksum validation (`shasum -a 256 -c`)  
- **Notes**:
  - Court bundle = index on page 1 (file this one)  
  - Searchable bundle = for reading/searching only  
  - Release automated via `nova_release` function  
