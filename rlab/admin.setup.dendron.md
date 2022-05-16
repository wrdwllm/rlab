---
id: wgcpbxt6jiq9b4vp8dnqvho
title: Dendron
desc: ''
updated: 1647063889865
created: 1647062070862
---

## Setting up Dendron

1. Install [Visual Studio Code](https://code.visualstudio.com/download)
2. Install [git](https://git-scm.com/) (Windows only)
   1. [Add `git` to Windows PATH](https://stackoverflow.com/questions/26620312/git-installing-git-in-path-with-github-client-for-windows)
3. Install [Dendron](https://marketplace.visualstudio.com/items?itemName=dendron.dendron)
   1. Open the command palette using <kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>
   2. Create a new [workspace](https://wiki.dendron.so/notes/c4cf5519-f7c2-4a23-b93b-1c9a02880f6b/) using `> Dendron: Initialize Workspace`
4. [Make a GitHub account](https://github.com/join)
   1. Send username to @wrdwllm
   2. Accept invitation to the [winter-intensive](https://github.com/wrdwllm/winter-intensive) repository
5. [Link GitHub to VS Code using the GitHub extension](https://code.visualstudio.com/docs/editor/github)
6. Install required extensions
   1. [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
   2. [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
   3. [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)
   4. [Dendron Markdown Shortcuts](https://marketplace.visualstudio.com/items?itemName=dendron.dendron-markdown-shortcuts)
   5. [GitHub Pull Requests](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
   6. [Dendron Paste Image](https://marketplace.visualstudio.com/items?itemName=dendron.dendron-paste-image)
7. Initialise a remote Dendron vault using the GitHub link
   1. Run `> Dendron: Add Vault`
   2. Select `remote`
   3. Paste <https://github.com/wrdwllm/winter-intensive.git> and press <kbd>Enter</kbd>
8. Add content and sync with remote repository
   1. Pull most recent commit when you open Dendron
      1. Open terminal shell
      2. Navigate to root workspace directory with `.git` (not vault)
      3. ![Screenshot](/assets/images/2022-03-12-16-35-12.png)
      4. Run `git pull`
   2. Push to remote after making significant updates
      1. `git add .`
      2. `git commit -m 'commit message`
      3. Resolve conflicts using the Source Control tab (contact @wrdwllm if unsure)
      4. `git push`

## Workflow

1. Follow the [Getting Started Guide](https://wiki.dendron.so/notes/678c77d9-ef2c-4537-97b5-64556d6337f1/) and the Dendron tutorial
2. Use [Markdown](https://wiki.dendron.so/notes/ba97866b-889f-4ac6-86e7-bb2d97f6e376/)
3. Make a new note
      1. Press <kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>L</kbd>
      2. Write content
      3. [Link to a note](https://wiki.dendron.so/notes/3472226a-ff3c-432d-bf5d-10926f39f6c2/) using syntax `[[note.file.name]]`
      4. Open Markdown preview window using `> Dendron: Show Preview`
      5. Use [GitHub Flavoured Markdown](https://wiki.dendron.so/notes/8DCgctK-RMD4EeHjC5_hI/)
      6. Resolve display issues with `> Dendron: Reload Index` and `> Developer: Reload Window`
4. Sync to repository (see Step 8 in previous section)
