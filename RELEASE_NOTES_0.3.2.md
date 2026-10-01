# VersoFold 0.3.2

October 1, 2026 · macOS 13 or later (Apple silicon and Intel) · Linux x64

VersoFold now runs on Linux, and connected agents like Claude Code and Codex are much easier to use.

## VersoFold for Linux

- A `.deb` package for Ubuntu and Debian, and an AppImage for other distributions, both x64.
- The same app as on macOS: the built-in LaTeX (pdfLaTeX, XeLaTeX, LuaLaTeX, BibTeX, SyncTeX) and history tools come bundled, so nothing else needs installing.
- Agent commands run in a bubblewrap sandbox, the Linux counterpart of the macOS one. Remembered API keys and sign-ins are protected by your system keyring (GNOME Keyring or KWallet).
- Shortcuts read Ctrl and Alt on Linux and Windows, in the app and in the handbook, including for coauthors who join in a browser.

## Connected agents, simplified

- **One model menu.** Claude Code, Codex and any ACP agent now sit in the agent panel's **Choose model** menu, under **Connected agents**, next to your other models. Choose one to chat with it; choose a model to switch back. One history holds both kinds of conversation.
- **Set up in one click.** Settings → External agents → **Use VersoFold from another app** adds VersoFold to Claude Code, Codex, Claude Desktop or Cursor with one click: nothing to copy, no configuration file to find. **Remove** takes it out again.
- **Missing agents explain themselves.** If Claude Code or Codex is not installed, the menu says so and the chat shows how to install it and sign in.
- **Attach images and files.** Connected chats get the **+** menu: images and text files, the selected passage, and the prompt library.

## Downloads

The macOS DMGs contain the Developer ID-signed, Apple-notarized app. Open the DMG for your Mac and drag VersoFold into Applications. Existing installs update from within the app.

On Ubuntu or Debian, install the `.deb` with `sudo apt install ./VersoFold-0.3.2-x64.deb`. On other distributions, make the AppImage executable and run it (Ubuntu also needs `sudo apt install libfuse2t64` for AppImages). The Linux packages are not signed.

| Computer | Installer | SHA-256 |
| --- | --- | --- |
| Mac, Apple silicon | `VersoFold-0.3.2-arm64.dmg` | `3973c74373ab907f3cd001d8d23642b8392913398a3610ad284e9168ede57d56` |
| Mac, Intel | `VersoFold-0.3.2-x64.dmg` | `ea3904fa32294d37c55de25b0becce451e788bcbd48fa5439033d108d6c2952d` |
| Linux x64, Ubuntu/Debian | `VersoFold-0.3.2-x64.deb` | `af44d231c911874ca5204b5e4e03ae362469bd64d209cb82fc19d9bcd97a317c` |
| Linux x64, other | `VersoFold-0.3.2-x64.AppImage` | `3d545cfc9af1dfbbc5f65f75ed7dc7eefc79bb3b8ef3e3242f4801b80cf00afc` |

The ZIP files, blockmaps, `latest-mac.yml` and `latest-linux.yml` support in-app updates.

The official desktop app remains free to use under the [VersoFold Desktop Software License](https://versofold.com/versofold-license.txt). Your documents remain yours; see the [third-party notices](https://versofold.com/third-party-notices.txt) for included components.
