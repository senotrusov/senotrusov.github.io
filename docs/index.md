---
hide:
  - feedback
---

# Stanislav Senotrusov

## Notes I couldn’t keep to myself

* [Installing Arch Linux](/notes/installing-arch-linux/)

## Handy tools I’ve made

### etcdotica: dotfiles and system config management

[**etcdotica**](https://github.com/senotrusov/etcdotica) is a lightweight tool that keeps selected system configuration files synchronized with a Git repository by acting as a file-level overlay, in which the repository serves as the source of truth while untracked files on the system remain untouched.

It mirrors tracked files directly to their corresponding paths without translation layers, supports collecting local edits back into the repository, and can watch for changes to apply updates automatically.

It can inject user-managed sections into existing machine- or distribution-specific system configuration files, appending and maintaining only the designated blocks while preserving the rest of the file exactly as provided by the system.

Overall, it offers a predictable way to manage configuration in plain text with minimal abstraction.

### Copy and Paste Tabs for Firefox

[**Copy and Paste Tabs**](https://addons.mozilla.org/en-US/firefox/addon/copy-and-paste-tabs/) is a lightweight [Firefox](https://www.firefox.com/) extension for quickly copying open tabs to the clipboard and reopening multiple URLs by pasting them back.

It can copy tabs from the active window, selected tabs, or all windows, and export tab titles and links in several formats, including Markdown, LaTeX, and MediaWiki.

When pasting text, it can extract URLs from a wide range of markup styles and recreate windows based on section headers in the markup.

It is especially useful for archiving research sessions, saving link collections in notes, or sharing groups of tabs.
