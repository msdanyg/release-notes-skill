# Example input

> **Illustrative — all data below is invented.** No real product or release is described.

**Request:** Write release notes from these eng notes. Audiences: admins and end users. Our docs say "workspace" (not "project") and "team insights" (not "analytics dashboards").

**Raw engineering notes (as received):**

```
- Added scheduled exports. Users can schedule CSV/PDF export of any team insights view
  (daily/weekly/monthly). Runs under the requesting user's permissions. Config in
  workspace settings > exports.
- BREAKING-ish: new permission scope "exports:manage". Existing admin roles get it
  automatically at migration; custom roles DO NOT and must be updated manually or
  scheduled exports won't be visible to those users. Migration runs with the release.
- Fixed: weekly digest email showed stale team names after a team was renamed
  (cache wasn't invalidated). Now reflects renames within 15 min.
- Improved sync performance.
```
