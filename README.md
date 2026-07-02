# combinatorics

## Automated PDF build

This repository builds its LaTeX PDFs with a cross-platform Python wrapper around `latexmk`.
Generated PDFs are ignored by git and are published by GitHub Actions on every push.

Build all PDFs locally:

```bash
python scripts/build.py
```

Clean and create a release zip:

```bash
python scripts/build.py --clean --package
```

Outputs:
- `out/1_8.pdf`
- `out/2_5.pdf`
- `out/3_3_7.pdf`

The release zip is written to `dist/combinatorics-release.zip` and contains the PDFs plus a buildable source tree.

