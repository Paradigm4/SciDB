# Branch and tag naming convention for P4 Github repos

The following is a proposal for branch and tag naming strategy for Paradigm4 plugins (e.g. accelerated_io_tools) and repositories (e.g. Shim).

- **Branches**: Versions of plugins that work on old SciDB versions should branch off at vXX.Y (e.g. v15.7, v15.12). 
- **Master branch**: The version of plugin that works on latest version of SciDB (and active development) is 
at master. So while SciDB is current at `18.1`, there should be no `v18.1` branch for any plugin.
- **Release tags**: Now plugins must be shipped to customer for old or current versions of SciDB. 
Proposal is to create `relXX.Y.Z` (where `XX.Y` is the scidb version, and `Z` is the minor releases numbered `1, 2, ...`). 
It is OK if we use `vXX.Y.ZZ` here instead of release. 
If we decide to go this route, then the change needs to be made in all the plugins where `relXX.Y.Z` is used.
- **Use of tags for extra-scidb-libs**: Only tags should be used for building `extra-scidb-libs` ([here](https://github.com/Paradigm4/extra-scidb-libs/blob/master/extra-scidb-libs.sh#L89)). Otherwise if a branch is used, we can easily break the build by pushing a change to that commit. Everytime a new tag is referenced in `extra-scidb-libs`, the minor version of `extra-scidb-libs` should be bumped up. 

## Edit to old naming convention

Earlier naming strategy was not consistenet -- `vXX.Y` was sometimes used for a branch, and sometimes used for a release. 
Compare for example https://github.com/Paradigm4/shim/branches with https://github.com/Paradigm4/shim/tags -- 
`v15.12` refers to a branch, while `v15.7` was a tag. 

Any tags with `vXX.Y` should probably be renamed to `vXX.Y.Z`
