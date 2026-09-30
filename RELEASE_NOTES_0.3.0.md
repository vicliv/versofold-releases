# VersoFold 0.3.0

September 30, 2026 · macOS 13 or later · Apple silicon and Intel

VersoFold 0.3.0 is about working together: live co-editing with named cursors, Overleaf-style track changes, automatic two-way sync with Overleaf, and agents that do real work and tell you when they need you.

## Write together

- Everyone with a file open edits the same document live, with named, coloured cursors and selections. A chip per person sits in the header; click one to jump to their cursor. Typing during a dropped connection merges when it returns, and ⌘Z undoes only your own edits.
- **Track changes** (⌘⇧E) records edits in each author's colour. Hover a change to accept or reject it, and step through changes with ⌘⌥] and ⌘⌥[. The **Review** tab (⌘⇧R) filters by author, file and kind, and accepts or rejects in bulk. A **Suggest** link lets a coauthor propose tracked changes only.
- Agents' edits arrive as tracked changes in their own names, with a link back to the conversation that made them.

## Overleaf, both ways, automatically

- Turn on **Sync automatically** (Publish → Overleaf sync) and a workspace stays in step with its Overleaf project through Overleaf's Git bridge. It syncs every few minutes, shortly after you edit, or when you press **Sync now**, while coauthors keep writing on Overleaf.
- Edits on both sides are merged line by line. When you and a coauthor change the same lines, that file waits on both sides until you choose **Keep mine** or **Keep Overleaf's**, and every other file keeps syncing. Nothing is overwritten or force-pushed.
- The first sync finds the Overleaf version a downloaded project started from, so edits made on both sides since then merge cleanly.

## Agents that work, and tell you when they need you

- The built-in agent edits in **Edit** mode by default. It can read and write any text file in the paper, create and move files, and run commands in a sandbox that cannot leave the workspace. A request that needs more access pauses and asks instead of failing. **Plan** and **Discuss** stay read-only.
- Connect Claude Code, Codex or any MCP client from **External agents**. Connections have edit access by default, and a missing permission is one click to grant.
- **Notifications** tell you when an agent needs approval, asks a question or finishes. You get a system notification while VersoFold is in the background, plus a bell with a count in the header and on the Dock icon.

## References

- Reviewing a checked reference is one screen: the record, the fields checked, sources, corrections as before → after, and one-click **Confirm** or **Apply correction**. A queue steps through every record that needs review.
- A `.bib` entry with unbalanced braces is reported and skipped, instead of silently dropping every entry after it. Publisher links from Nature, Springer, ACM, Science and ACL Anthology now fill in their metadata.

## A Visual editor that looks like the PDF

- The Visual editor measures the last build's PDF: page and margins, fonts, headings, captions, citations and numbering read as printed. It draws tables, pseudocode, theorems, a document's own macros, and `\input` files in place, where you can edit them.
- Typing redraws only the paragraph you are in, so long papers stay fast.

## Fixes

- The first build of a paper with citations no longer shows warnings that a later pass resolved.
- Typing keeps saving while a PDF builds.
- The version history can no longer take in its own files, which previously left every build marked "out of date". A history already affected repairs itself at the next snapshot.
- Show in PDF works from text in `\input` files. PDF figures made with standard fonts show their labels in the preview.
- Keyboard focus stays inside dialogs and returns to what opened them.
- An agent request that stops responding is retried once and then reported, instead of waiting indefinitely. Agents can read a paper's record at doi.org, Crossref or arXiv when checking a reference, so the corrections they find arrive as one-click proposals.
- Remote folders over SSH start in your home folder, and a missing folder says so plainly.
- The desktop app keeps a stable local port, so layouts and preferences survive relaunches.
- Many layout, copy and menu fixes across the side panels, in both themes.

## Downloads

Both downloads contain the Developer ID-signed, Apple-notarized VersoFold app. Open the DMG for your Mac and drag VersoFold into Applications. Existing installs update from within the app.

| Mac | Installer | SHA-256 |
| --- | --- | --- |
| Apple silicon | `VersoFold-0.3.0-arm64.dmg` | `be945ad2cb6d623eac92787de438a9649d220e02cce8e221100285da674d5fac` |
| Intel | `VersoFold-0.3.0-x64.dmg` | `744a51dc5a7e89af2e1b7eab395d5ab0bccdba1e70296abc6751fdf52ff1fb5b` |

The ZIP files, blockmaps, and `latest-mac.yml` support in-app updates. Choose the DMG matching your Mac for a direct installation.

The official desktop app remains free to use under the [VersoFold Desktop Software License](https://versofold.com/versofold-license.txt). Your documents remain yours; see the [third-party notices](https://versofold.com/third-party-notices.txt) for included components.
