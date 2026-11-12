# WebCode

A static, in-browser code editor: CodeMirror 6 + SolidJS + Vite. No server, no accounts, every feature free.
Files live in your browser (IndexedDB). Works offline once loaded (PWA) and can be installed on iPad / desktop.

## Build

    npm install
    npm run build      # static site in ./dist
    npm run dev        # local dev server

## Host on GitHub Pages
Publish the contents of `dist/` (a `gh-pages` branch or a `docs/` folder). All paths are relative,
so it works at https://user.github.io/repo/. Open it once online; after that it is cached for offline use.

## Features
- Editor: ~40 languages (loaded on demand), find/replace (regex, case, word), multi-cursor, column select, folding,
  bracket matching/auto-close, autocomplete (words + snippets, Emmet for HTML/CSS), minimap, Vim mode,
  whitespace display, line tools (sort, join, trim, case, duplicate/delete line), go to line / symbol.
- Workspace: virtual filesystem, explorer, tabs, split panes, quick open (Ctrl/Cmd+P), command palette
  (Ctrl/Cmd+Shift+P), search and replace across all files, session restore, drag and drop upload.
- Archives: extract zip / tar / tar.gz, download any folder as .zip or .tar.gz (runs in a Web Worker).
- Tools: diff / compare two files, local file history with restore, live preview for HTML (with console),
  Markdown, SVG, JSON, images and PDF.
- Touch: key row (Tab, arrows, brackets, symbols) and mobile-friendly input settings.

## Shortcuts
Ctrl/Cmd: S save, P quick open, Shift+P commands, Shift+F search files, Shift+O symbols, B sidebar, \ split.
