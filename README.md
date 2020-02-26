# Global installation instructions: (requires git 2.9 or later)

NOTE: if you configure core.hooksPath, then git only runs the hooks from that directory (and ignores repo-specific hooks in .git/hooks/), but these pre-commit hooks contain a block at the end which executes a repo-specific pre-commit hook if it's present. It's a small hax that I think is pretty nice.

1. `mkdir ~/.githooks`
2. `git config --global core.hooksPath ~/.githooks`
3. `cp pre-commit ~/.githooks/`
4. `chmod +x ~/.githooks/pre-commit`

# Uninstall:
`rm ~/.githooks/pre-commit`

