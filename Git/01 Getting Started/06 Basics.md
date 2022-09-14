# Gitignore
For a list of patterns that can be used in `.gitignore` files, see [this link](https://git-scm.com/docs/gitignore#_pattern_format) or [Atlassian gitignore guide](https://www.atlassian.com/git/tutorials/saving-changes/gitignore).

# VScode as difftool
To make VS Code your default “everything”, first you need to ensure you can run VS Code from the command-line.

Then, run the command `git config --global --edit` to edit the global config, and add the following:
```
[core]
  editor = code --wait
[diff]
  tool = vscode
[difftool "vscode"]
  cmd = code --wait --diff $LOCAL $REMOTE
```

If you already have `[core]` section, just add the `[diff]` and `[difftool]` sections to it.
