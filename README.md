# Bundle Artifacts Action
GitHub Action that bundles multiple workflow artifacts into a single artifact and uploads it to the current workflow.

## How to use?

```yaml
- name: Bundle Validation Artifacts
  uses: lasselundstenjensen/bundle-artifacts@main
  with:
    input_artifact_names: 'manual-test-results-validation-iv,manual-test-results-validation-pv'
    output_artifact_name: 'manual-test-results-validation'

- name: Bundle Production Artifacts
  uses: lasselundstenjensen/bundle-artifacts@main
  with:
    input_artifact_names: 'manual-test-results-production-piv,manual-test-results-production-ppv'
    output_artifact_name: 'manual-test-results-production'
```
