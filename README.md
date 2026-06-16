# spm-repo
The official repo that comes with spm by default. You can build more repositories off of this one or submit your own packages to be used in the official repo.
# Repository Structure
SPM repositories follow this structure: `{url to repo root}/{moldy os version number}/{architecture}/{package install candidate found in packagelist.json for the package name}/package.json`

For example, `https://github.com/olliequaas/spm-repo/1/x86_64/testpkg/package.json`

The file packagelist.json contains data about the repository SPM looks through. There, it can find the install candidate folder for the package you are installing, the default version (the version SPM automatically installs unless you specify a version), and more metadata. The file package.json in each install candidate folder contains dependencies of the package and their respective versions, pre and post install/uninstall script paths, and the package archive, normally in *.tar.gz format.
