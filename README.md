# git-hooks
Git hooks to help your project be better.

To make git run unit tests and lint tests, softlink the `pre-commit` and
`prepare-commit-msg` files into the `.git/hooks directory` of the repo you want
to test.  The following commands will get that done:
```bash
  ln --symbolic --force ../../git-hooks/pre-commit .git/hooks/pre-commit
  ln --symbolic --force ../../git-hooks/prepare-commit-msg .git/hooks/prepare-commit-msg
```

# Python requirements
`$ [sudo] pip install -r requirements-python.txt`

# Currently supported languages for linting

- Python
- Go
- Shell
