# Building Electron from Source

We are working from a fork of <https://github.com/electron/electron>, <https://github.com/psiservices-ccounterman/electron>

## Keeping fork in sync with upstream

This must be done each time the <https://github.com/psiservices-ccounterman/electron> repository is cloned.
See <https://help.github.com/articles/working-with-forks/>

```bash
git remote add upstream https://github.com/electron/electron.git
git fetch upstream
git checkout master
git merge upstream/master
git push
```

After that:

```bash
git fetch upstream
git checkout master
git merge upstream/master
git push
```

For other branches, e.g. "7-0-x":

```bash
git remote remove upstream
git checkout 7-0-x
git remote add upstream https://github.com/electron/electron.git
git fetch upstream
git merge upstream/7-0-x
git push
```

