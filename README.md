# Gitignore Generator Pro

[![CI](https://github.com/kasapdev/gitignore-generator-pro/actions/workflows/ci.yml/badge.svg)](https://github.com/kasapdev/gitignore-generator-pro/actions/workflows/ci.yml)

Generate merged, de-duplicated `.gitignore` files from 26 curated stack templates — fast, private, and fully offline.

> A premium, zero-dependency `.gitignore` builder. Every template — Node, Python, Unity, Godot, Docker, and more — is baked directly into the app as static text, so nothing is ever fetched from a network. Pick your stacks, watch the merged file build live, and copy or download a clean, de-duplicated result.

## Overview

Gitignore Generator Pro is part of the **Web Utility Suite**. It runs entirely in the browser with no build step, no frameworks, and no network calls — open `index.html` from disk and it works, even without an internet connection. A checkbox grid groups 26 real-world stacks by category; selecting any combination instantly rebuilds a single merged `.gitignore` in the preview pane, with each contributing stack labeled by a `# ==== Stack Name ====` header and every duplicate ignore pattern removed so the same line never appears twice.

## Features

- **26 curated templates** across six categories — Languages & Runtimes (Node.js, Python, Java, Go, Rust, C/C++ CMake, Ruby, PHP, .NET/Visual Studio, Elixir, Android, Xcode/Swift, Flutter/Dart), Frameworks & Engines (Unity, Godot, Next.js/React), Editors & IDEs (VS Code, JetBrains/IntelliJ, Sublime Text, Vim/Emacs), Operating Systems (macOS, Windows, Linux), DevOps (Docker, Terraform), and Environment & Secrets (`.env`, logs, keys).
- **Live merged preview** — every checkbox toggle instantly rebuilds the combined `.gitignore` text.
- **Smart de-duplication** — patterns already emitted by an earlier-selected stack are skipped everywhere they recur; a stack's header comment is only printed if it actually contributes a new line.
- **Search/filter box** — narrow the checklist by stack name as you type.
- **Select all / Clear all** — one click to toggle every stack.
- **Copy** to clipboard or **Download** as a real `.gitignore` file.
- **Auto-persist** — your last selection is saved to `localStorage` and restored on your next visit.
- **Dark & light themes**, fully responsive down to small screens, accessible, and keyboard-driven.

## Installation

No dependencies, no build step.

```bash
git clone https://github.com/kasapdev/gitignore-generator-pro.git
cd gitignore-generator-pro
```

Then simply open `index.html` in any modern browser (double-click it, or `file://` it). That's it.

## Usage

1. Use the **search box** to find a stack, or scroll the grouped checklist (Languages, Frameworks/Engines, Editors/IDEs, OS, DevOps, Environment & Secrets).
2. Check the boxes for every stack, tool, and OS relevant to your project.
3. Watch the **Preview** pane rebuild live — each selected stack appears as its own labeled, de-duplicated block.
4. Click **Copy** to copy the merged file to your clipboard, or **Download** to save it as `.gitignore`.
5. Your selection is remembered automatically — reopen the app later and it picks up where you left off.

## Keyboard Shortcuts

| Action                     | Shortcut                       |
| --------------------------- | ------------------------------ |
| Copy merged `.gitignore`    | <kbd>Ctrl/⌘</kbd> + <kbd>C</kbd> |
| Download `.gitignore`       | <kbd>Ctrl/⌘</kbd> + <kbd>S</kbd> |
| Show shortcuts help         | <kbd>?</kbd>                    |
| Close dialog                | <kbd>Esc</kbd>                  |

## Screenshots

> _Screenshots coming soon._

## Roadmap

- [ ] Per-stack "preview only this block" toggle before adding it to the merge
- [ ] Custom user-added patterns section appended to the generated file
- [ ] Import an existing `.gitignore` and detect which templates it roughly matches
- [ ] Shareable URL that encodes the current stack selection
- [ ] Additional templates (Kotlin, Scala, Haskell, WordPress, Laravel-specific)

## License

MIT Licensed. Part of the [Web Utility Suite](https://github.com/kasapdev/web-utility-suite).
