---
hide:
  - feedback
---

# Stanislav Senotrusov

## Notes I couldn’t keep to myself

* [Installing Arch Linux](/notes/installing-arch-linux/)

## Handy tools I’ve made

### `envfold` environment variable manager (2026)

(**envfold**](https://github.com/senotrusov/envfold) is a high-performance environment variable manager that replaces scattered `.env` files with a single, centralized configuration. It automatically applies and removes variables based on the current location in the filesystem, using pure shell logic rather than spawning external processes on each directory change. This approach maintains shell responsiveness while keeping project directories clean and enabling precise, context-aware environment control.

At shell startup, `envfold` compiles its configuration into optimized native shell code, allowing instant evaluation on every directory change. It supports hierarchical inheritance, dynamic value resolution with optional caching, and convenient variable manipulation such as `PATH` prepending.

Manual overrides defined interactively in the shell are preserved and remain in effect even after leaving a directory.

### Copy and Paste Tabs for Firefox (2026)

[**Copy and Paste Tabs**](https://addons.mozilla.org/en-US/firefox/addon/copy-and-paste-tabs/) is a lightweight [Firefox](https://www.firefox.com/) extension for exporting tab titles and URLs to the clipboard and restoring sessions from pasted URL lists.

Tab titles and URLs can be copied from the active window, selected tabs, or all windows, with options to include or exclude pinned tabs. Pasted text opens every valid link as a new tab, either in the current window or in newly created windows.

Links can be copied in plain text, AsciiDoc, LaTeX, Markdown, MediaWiki, Org mode, reStructuredText, and Textile. When text is pasted, URLs can be extracted from many markup formats, and multiple windows can be recreated based on section headers in the markup.

This makes it useful for archiving and restoring research sessions, saving link collections in notes, or sharing tabs in messages.

### etcdotica: dotfiles and system config management (2025)

[**etcdotica**](https://github.com/senotrusov/etcdotica) is a lightweight tool that keeps selected system configuration files synchronized with a Git repository by acting as a file-level overlay, in which the repository serves as the source of truth while untracked files on the system remain untouched.

It mirrors tracked files directly to their corresponding paths without translation layers, supports collecting local edits back into the repository, and can watch for changes to apply updates automatically.

It can inject user-managed sections into existing machine- or distribution-specific system configuration files, appending and maintaining only the designated blocks while preserving the rest of the file exactly as provided by the system.

Overall, it offers a predictable way to manage configuration in plain text with minimal abstraction.
