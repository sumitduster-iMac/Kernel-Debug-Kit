# Automation Scripts

This directory contains automation scripts for the Kernel Debug Kit repository.

## check_kdk_releases.py

Automated script to check for new Kernel Debug Kit releases from Apple.

### Usage

```bash
python3 scripts/check_kdk_releases.py
```

### Features

- Checks for new KDK releases from Apple
- Tracks versions in `kdk_versions.json`
- Integrates with GitHub Actions for automated checks
- Creates notifications when new releases are detected

### Requirements

```bash
pip install requests beautifulsoup4 lxml
```

### GitHub Actions Integration

This script is automatically run daily via the `.github/workflows/check-kdk-updates.yml` workflow.

### Note

Full automation requires Apple Developer credentials for accessing the download catalog. The current implementation provides a framework for manual verification and tracking.
