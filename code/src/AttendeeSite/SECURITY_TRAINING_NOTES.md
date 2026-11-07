# Dependency security training notes

This is an isolated GitHub Skills sample repository. It is **not production software**.

## Critical minimist remediation

- Detected the Dependabot advisory for prototype pollution affecting minimist versions below 1.2.6.
- Updated the sample project's declared dependency from `^1.2.5` to `^1.2.8`.
- Updated the lockfile's resolved minimist tarball and integrity using npm registry metadata.
- Reviewed and merged the focused security pull request.
- Keep Axios and follow-redirects findings open until the appropriate subsequent course steps; do not deploy this sample.

## Repeatable review checklist

1. Confirm the advisory's affected range and earliest patched version.
2. Keep the dependency manifest and lockfile consistent.
3. Review the patch and run available validation.
4. Merge and verify the Dependabot alert state, then re-scan.
