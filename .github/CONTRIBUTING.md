# Contributing

Thank you for investing your time in contributing to this project, even if you report a bug, fix a typo, or develop a new feature!  

Please read the [Code of Conduct](https://raw.githubusercontent.com/actforgood/.github/main/CODE_OF_CONDUCT.md).  
Please be aware that PRs should be submitted with an agreement like:
> *Contributor License Agreement*  
> By submitting this pull request, I confirm that my contribution is made under the terms of project's license.


## Setup
Fork the project to your personal GitHub account, then clone the project:
```bash
mkdir -p $GOPATH/src/github.com/actforgood
cd $GOPATH/src/github.com/actforgood
git clone git@github.com:your_github_username/some_actforgood_project.git
cd some_actforgood_project
git remote add upstream https://github.com/actforgood/some_actforgood_project.git
git fetch upstream
```

Run a `make all` to check everything is ok.

## Making Changes

Start by creating a new branch for your changes:

```bash
git checkout main
git fetch upstream
git rebase upstream/main
git checkout -b feature_xyz
```

Before pushing, make sure everything is ok by running a `make all`.

For a PR to be more likely to be accepted, make sure:
- you cover with (unit /& integration) tests the code you're writing (`make cover`).
- you add meaningful comments to your code
- you add examples, if applicable
- you change the documentation/Readme, if applicable
- you add benchmarks, if applicable
- you add 3rd party dependency's license in the dedicated area in Readme, if applicable
- you maintain backward compatibility
- write a meaningful commit message

Then you can push the changes to your repository.
```bash
git push origin feature_xyz
```

Open a PR through GitHub UI. At this point, wait for your PR to be reviewed.  
Thank you for contributing!  