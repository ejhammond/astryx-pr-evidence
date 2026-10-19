# Prebuilt Astryx data-color reproduction

These are production Vite builds with no StyleX compiler, using the compiled public `dataVars` entry and prebuilt Core + Neutral theme CSS.

- Before: published `@astryxdesign/core@0.7.1` and `@astryxdesign/theme-neutral@0.7.1`.
- After: Core packed from the proposed distribution-build fix, with the same published Neutral CSS.
- Both raw `var(--color-data-categorical-blue)` and the compiled `dataVars` import are transparent before and canonical blue after.
- Light/dark and both physical stylesheet orders are captured; the authored blue theme override remains unchanged.
- `measurements.json` contains independently asserted computed browser colors; `size.json` records the retained group's size.

Images are kept in this separate public repository, never in the Astryx pull-request branch. No internal links, hostnames, or operational context are included.
