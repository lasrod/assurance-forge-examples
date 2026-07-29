# GSN Pattern Decorators

A focused manual-test project for GSN pattern element-abstraction notation.

## Open

In Assurance Forge, select **File → Open Project** and open:

```text
projects/gsn-pattern-decorators/af.proj
```

## Expected result

The GSN canvas contains two goals:

- `G1: Uninstantiated Goal` has a hollow triangle below the goal;
- `G2: Undeveloped Pattern Goal` has a horizontally bisected hollow diamond,
  representing the combined undeveloped and uninstantiated state.

Select **File → Export → GSN SVG** and confirm the exported diagram contains
the same markers.

Select G1 and enable **Undeveloped** in **Element Properties** to exercise the
library-backed edit bridge: its hollow triangle should become a bisected
diamond. Save and reopen the project to verify persistence.
