# Setup migrations

Re-sync is an in-place schema repair, not a second setup. Read the existing charter, index, log,
hub notes, baton, queue, and business files before proposing a patch. Founder-authored prose, custom
laws, history, raw sources, and unknown files survive byte-for-byte unless the founder explicitly
approves a content edit.

Every supported re-sync copies the plugin's `scripts/graph-audit` into the vault byte-for-byte,
preserves executable mode, and runs graph-audit before advancing the version marker. Validator
failures stay visible and keep the migration incomplete.

## Detect the version

Read `.co-founder-version` at the business-folder root.

- `1.0.0`: verify the current scaffold with the graph gate below and replace only missing or
  byte-different validator code.
- No marker plus a co-founder-shaped charter/vault: treat the vault as damaged. Propose the graph
  gate below as a repair and get the founder's explicit yes before writing anything.
- Any other value: report the unknown migration and stop without writing.

## Re-sync graph gate

Build one proposed patch, show it, get the founder's explicit yes, then apply in this order:

1. **Shipped validator.** Copy `graph-audit` into `scripts/` with executable mode.
2. **Machine baton.** Add the fixed baton frontmatter from `vault-scaffold.md`. Derive active
   path, state, roadmap counts, next step, and content projections from canonical files. A conflict
   stays unresolved for graph-audit; it is not guessed into agreement.
3. **Catalog projections.** Add `[state: ...] [roadmap: ...]` to initiative index rows,
   put each initiative under one exact state bucket, and add content-state tokens to index/business
   hub rows.
4. **Receipt fields.** Add vision strategy state, public-work receipt fields, and content
   approval/publication receipt fields. Missing evidence stays null/PARKED or requires the
   founder's exact confirmation captured in an immutable raw session receipt. Any decision page,
   offer term row, approval field, or `Founder's yes:` carries its immutable consent receipt or is
   not written (shared contract, Immutable consent receipts).
5. **Graph closure.** Run graph-audit across the complete vault. Reconcile stale baton, index,
   hub, event, queue, roadmap, `updated`, and receipt-anchor projections through exact approved lines.
6. **Close.** After graph-audit exits zero, append
   `## [date] resync | verified at 1.0.0` and write the `1.0.0` marker. Rerun graph-audit once
   after that final event. A second re-sync proposes nothing.

Done when: one vault remains, founder prose and history are preserved, graph-audit exits zero,
the marker reads `1.0.0`, and a second re-sync proposes no changes.
