# gitea-sync-test
___
This is a sample readme, version 1 - Before setting up a mirror to Gitea
Push test
2323
# Notes
1. Mirrors are read only
2. Mirrors can be changed into local repositories, and set as push repositories to gh. If this is done, any change to gitea will be pushed to gh, but as a forced change. So, if someone changes something in gh, and something in gitea, the file will be overwritten. In this scenario, files in gh will also not be pulled from the repo.
3. Ideally, gh repos should be push only, and all changes should happen in gitea. This way we have a local git, while still using some features to push to gh for CF Pages to use.
In this case, the workflow will look like this (directions of arrows matter):
Dev client <-> Gitea (all git-related) -> Github (main) => GH Pages

