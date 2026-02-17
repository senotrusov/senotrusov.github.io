---
hide:
  - feedback
---

# Stanislav Senotrusov

## Notes I couldn’t keep to myself

* [Installing Arch Linux](/notes/installing-arch-linux/)

## Handy tools I made

### etcdotica: dotfiles and system config management

[**etcdotica**](https://github.com/senotrusov/etcdotica) is a lightweight tool that keeps selected system configuration files synchronized with a Git repository by acting as a file-level overlay, in which the repository serves as the source of truth while untracked files on the system remain untouched.

It mirrors tracked files directly to their corresponding paths without translation layers, supports collecting local edits back into the repository, and can watch for changes to apply updates automatically.

It can inject user-managed sections into existing machine- or distribution-specific system configuration files, appending and maintaining only the designated blocks while preserving the rest of the file exactly as provided by the system.

Overall, it offers a predictable way to manage configuration in plain text with minimal abstraction.
