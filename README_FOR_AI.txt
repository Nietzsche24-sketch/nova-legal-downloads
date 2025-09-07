# Tachyon Anchor

# NovaLegal Tachyon Anchor

This file tracks all releases (Atlas bundles) in chronological order.
Each entry includes tag, assets, verification, and notes.

---
## Release: Smith v Ontario — Application Record
**Tag**: v2025.09.07-app3  
**Date**: 2025-09-07  
**Bundles**:  
- smith_full_bundle.zip — Court bundle + Searchable bundle + README  
- smith_review.zip — Searchable-only + README  

**Checksums**:  
- SHA256SUMS.txt uploaded with both ZIPs  

**Verification**:  
- Both zips passed checksum validation (`shasum -a 256 -c`)  

**Notes**:  
- Court bundle = index on page 1 (file this one)  
- Searchable bundle = for reading/searching only  
- Release automated via `nova_release` function  

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
---

## Release: [ClientName] — Application Record
**Tag**: vYYYY.MM.DD-appX  
**Date**: YYYY-MM-DD  
**Bundles**:  
- [client]_full_bundle.zip — Court bundle + Searchable bundle + README  
- [client]_review.zip — Searchable-only + README  

**Checksums**:  
- SHA256SUMS.txt uploaded with both ZIPs  

**Verification**:  
- [Pass/Fail] checksum validation (`shasum -a 256 -c`)  

**Notes**:  
- Court bundle = index on page 1 (file this one)  
- Searchable bundle = for reading/searching only  
- Release automated via `nova_release` function  
