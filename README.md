# semver-docker
auto tag docker images semver based on commit history using svu


### Pre-Requisties

- [svu cli]() installed


#### How it works?

- any PR request would build using shasum
- any merge on main uses `git tag $(svu next)` to tag and release


see ![workflow.yaml](./.github/workflows/workflow.yaml)