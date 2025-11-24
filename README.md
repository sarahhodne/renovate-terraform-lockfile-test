# renovate-terraform-lockfile-test

## Current behaviour

Enabling `lockFileMaintenance` on a repository with `required_versions` and a `.terraform.lock.hcl` file causes Renovate to open a PR that updates the `.terraform.lock.hcl` file to no longer match the `required_versions` constraint.

## Expected behaviour

`lockFileMaintenance` respects the `required_versions` constraint, and doesn't update past what that allows.

## Link to the Renovate issue or Discussion

Put your link to the Renovate issue or Discussion here.
