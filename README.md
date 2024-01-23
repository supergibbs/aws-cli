# aws-cli

Simple Amazon Linux with CLI pre-installed. Designed to be helpful when running multiple aws cli commands for CI/CD and avoid having to install CLI on each run.
The [official AWS CLI](https://gallery.ecr.aws/aws-cli/aws-cli) image uses an entrypoint making it hard to run multiple commands and is outdated.

Supports Amazon Linux 2 and 2023.

Installs the following:

- awscli (v2)
- jq
- findutils
- gzip