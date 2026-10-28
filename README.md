# Work Command Center · Web Demo

An English interactive demo using fictional data only. It demonstrates the original app’s workflow without including its database or backups.

## One-minute walkthrough

1. **Today:** star up to three daily focus items.
2. Complete **Summarise user feedback** and watch project progress update.
3. **Projects:** open **Customer portal refresh** to explore project → task → next action.
4. Click a task title to edit its status, target date, follow-up or 10-minute next step.
5. **Reports:** review and copy the updated summary.
6. **Reset demo:** start again with fresh fictional data.

## Behaviour and limits

- Static HTML/CSS/JavaScript, without external dependencies or a backend.
- Changes stay in your browser’s localStorage (`wcc-public-demo-en-v1`). Each visitor has an independent copy.
- The English demo uses separate storage from the earlier Hungarian demo. Existing Hungarian demo data is left untouched.
- Initial dates are relative to the first visit. Resetting generates fresh dates.
- Daily focus resets on a new day. The latest change can be undone until another change or page refresh.
- Completing a task with open next actions requires confirmation. The combined completion can be undone together.
- Project progress is the percentage of completed tasks and next actions. Milestones are tracked separately.
- Reports are current snapshots, not the original app’s full daily/weekly report module. Copying does not send anything.
- No imports, sign-in, analytics or data submission. Do not enter real or confidential data.

## GitHub Pages

**Settings → Pages → Deploy from a branch → main → / (root) → Save.**

All asset URLs are relative, so the app works at the repository’s Pages subpath.

## Local preview

Open `index.html` in a modern browser. For clipboard access and consistent local storage, serve the folder over HTTP, for example with `python3 -m http.server 8000`.
