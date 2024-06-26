# gitea-sync-test
___
This repo was initially set as a mirror from https://github.com/njwww/gitea-sync-test.git, but has been unlinked as a mirror and set as a push mirror to https://github.com/njwww/gitea-sync-test.git.
# Notes
1. Mirrors are read only
2. Mirrors can be changed into local repositories, and set as push repositories to gh. If this is done, any change to gitea will be pushed to gh, but as a forced change. So, if someone changes something in gh, and something in gitea, the file in gh will be overwritten with changes from gitea. In this scenario, files in gh will also not be pulled from the repo.
3. Ideally, gh repos should be push only, and all changes should happen in gitea. This way we have a local git, while still using some features to push to gh for CF Pages to use.<br>
In this case, the workflow will look like this (directions of arrows matter):<br>
Dev client <-> Gitea (all git-related) -> Github (main) => GH Pages

### Repos that may be affected by this change
- njwww-backend
- pages-njwyganowski-com
- cdn-backend

