# Terraform Beginner Bootcamp 2023

## Semantic versioning :mage:

The versioning will be based on standard semantic versioning [semver.org](https://semver.org/)

**MAJOR.MINOR.PATCH**, ie. `1.0.1`

- **MAJOR** version when you make incompatible API changes
- **MINOR** version when you add functionality in a backward compatible manner
- **PATCH** version when you make backward compatible bug fixes

## Install the Terraform CLI without interaction

### Verify the latest installation instructions

The Terraform CLI installation changes constantly. Read the documentation to ensure you have the latest.

[Install Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

### Refactoring Bash Scripts

Created a new bash shell script to keep the installation cleaner with `#!/bin/bash`

Scripts in .gitpod.yml, you need a program to interpret it

`source ./bin/install_terraform_cli`

https://en.wikipedia.org/wiki/Shebang_(Unix)

### Linux Permissions

The bash script should have execute permissions. To change them for the user context, use the following:
`chmod u+x file_name`


https://en.wikipedia.org/wiki/Chmod


### Execution without gitpod.yml

Execution is better served as before instead of init. The former is only executed with new workspaces but not with old.

https://www.gitpod.io/docs/configure/workspaces/tasks