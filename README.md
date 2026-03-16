# setup-ta-lib

Install the TA-Lib C library for use in GitHub Actions workflow.

## Usage

```yaml
jobs:
  test:
    runs-on: ubuntu-latest
    name: Install TA-Lib
    steps:
      - uses: actions/checkout@v3
      - uses: TA-Lib/setup-ta-lib@v1.0.1
```

This will automatically install the latest TA-Lib C release.

If you want to install a particular version, you can:

```yaml
  - uses: TA-Lib/setup-ta-lib@v1.0.1
    with:
      version: 0.6.4
```
