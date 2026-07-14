# Example output

> **Illustrative — generated from the invented notes in `example-input.md`.**

## Release notes — Admins

**Action required: new permission scope for scheduled exports.** This release adds an `exports:manage` permission scope. Built-in admin roles receive it automatically. **Custom roles do not** — update any custom role that should manage scheduled exports, or those users will not see the feature. The migration runs with this release.

**New: scheduled exports.** Users can schedule recurring exports (CSV or PDF) of any team insights view — daily, weekly, or monthly. Exports run under the requesting user's permissions and are configured in workspace settings under Exports.

**Fixed: stale team names in the weekly digest.** Renamed teams now appear correctly in digest emails within 15 minutes of the rename.

## Release notes — End users

**New: scheduled exports.** You can now schedule any team insights view to export automatically as a CSV or PDF — daily, weekly, or monthly. Set it up in workspace settings under Exports. If you don't see the option, ask your admin about access.

**Fixed:** the weekly digest email now shows the current team name after a team is renamed.

## Questions for engineering

1. **"Improved sync performance"** — improved for initial sync, incremental sync, or both? Measured how, and at what scale? Is the improvement visible to users (faster load) or infrastructure-side only? Held from the notes until answered — as written, it promises nothing a reader can verify.

## Channel variants

Want the changelog entry, the customer email, or the in-app announcement built from these notes?
