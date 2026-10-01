# VersoFold 0.4.0

October 1, 2026 · macOS 13 or later (Apple silicon and Intel) · Linux x64

VersoFold now knows where your paper is in its life, and the rebuttal moves into the editor: the reviewers' comments with your answers under them, written together with your coauthors. The preprint and the supplementary material are built from the same LaTeX as your submission.

## Paper phases

- Choose the paper's phase under its title: drafting, internal review, submission, under review, rebuttal or revision, camera-ready, published. The workspace follows it: the side panel's tabs, the checks that matter now, the agent's suggested starts. Nothing is locked.
- **Submission** asks where you are submitting, runs the venue's checklist and copies the title, abstract and keywords for the submission form. **Mark as submitted** saves the version the reviewers read.
- **Camera-ready** checks what usually goes wrong after acceptance: the authors still anonymous, the venue style's final option, the page limit, fonts not embedded, and each change promised in the rebuttal.
- **Published** copies a BibTeX entry for your own paper.

## The rebuttal, in the editor

- **Import reviews**: copy the whole OpenReview page and paste it. Each review arrives as labelled comments (W1, Q1…), word for word, with the ratings. Pasting again later adds only what is new, including the reviewers' replies to your rebuttal.
- **The Response view** opens beside the LaTeX: a general response to all reviewers, then each comment with your answer under it. Coauthors write in it with you, live, with their cursors. Each comment has a status, a decision, an assignee and **Draft with agent**, and each reply is counted against the reply limit.
- A formatting bar writes the Markdown OpenReview reads, with a live preview of your equations. The Response view can also have its own window.
- Edits since submission show in colour in the LaTeX and on the PDF, and a marked PDF (latexdiff) is one click away.
- **Copy for OpenReview** copies the general response or a reviewer's reply as Markdown. A journal revision downloads the whole response letter.

## Preprint & editions

- The named preprint and the supplementary material are built from the same LaTeX as your submission. Only what differs is marked, as plain LaTeX (`\ifpreprint … \fi`), so the paper still builds on Overleaf and arXiv.
- The button next to the phase switches the view between the paper and the preprint, for the PDF and the LaTeX. **Colour the differences** shows what the preprint adds; **Compare side by side** puts the two PDFs next to each other.
- Checks keep the submission anonymous and the preprint named. The arXiv package is built from the preprint, with text meant for other editions left out.

## Also new

- **Check the sources** replaces Evidence Lens: select a sentence and see the passages of the papers it cites.
- The agent has its own column, the side panel follows the paper's phase, and Snippets moved next to Bibliography and Figures.
- Connected Claude Code shows its exact models (such as Claude Sonnet 5), and each reply names the model that answered.
- Notifications work again in the desktop app: an agent's question, approval request or finished work reaches you while VersoFold is in the background. **Settings → General → Notifications** can send a test.
- **Settings → Your name & colour** sets the name and cursor colour your coauthors see.
- In split view, choosing a view replaces one pane and leaves the other alone. The PDF toolbar is quieter when the PDF is out of date.

## Downloads

The macOS DMGs contain the Developer ID-signed, Apple-notarized app. Open the DMG for your Mac and drag VersoFold into Applications. Existing installs update from within the app.

On Ubuntu or Debian, install the `.deb` with `sudo apt install ./VersoFold-0.4.0-x64.deb`. On other distributions, make the AppImage executable and run it (Ubuntu also needs `sudo apt install libfuse2t64` for AppImages). The Linux packages are not signed.

| Computer | Installer | SHA-256 |
| --- | --- | --- |
| Mac, Apple silicon | `VersoFold-0.4.0-arm64.dmg` | `9b45ae935e6599f1a47aee7a988c59143370fcf90b2fbba54949459b7342668c` |
| Mac, Intel | `VersoFold-0.4.0-x64.dmg` | `7e4ca143ad1ab170421436094f0ef7b5b0c740a60fdbf5024e1bf002e7904915` |
| Linux x64, Ubuntu/Debian | `VersoFold-0.4.0-x64.deb` | `809026324f2adab28e03b8e2bf97174d042096862b58eb00ce34f9a1b2715d6f` |
| Linux x64, other | `VersoFold-0.4.0-x64.AppImage` | `03e49e35c21c65c412938603d2cba9f48a3ebbb2828b577ac6a6e7a9ba434977` |

The ZIP files, blockmaps, `latest-mac.yml` and `latest-linux.yml` support in-app updates.

The official desktop app remains free to use under the [VersoFold Desktop Software License](https://versofold.com/versofold-license.txt). Your documents remain yours; see the [third-party notices](https://versofold.com/third-party-notices.txt) for included components.
