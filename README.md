# Auto-Action-Readme

Version: 1.1.0

Github Action to use the settings in action.yml to populate the readme.

## Usage

```yaml

- uses: ajparsons/auto-action-readme@cef8800ceae3c234db511988875475ed44d69802 # v1.1.0
  id: example-step 
  with:
    output_file: 'README.md'  # default
    commit_and_push: 'true'  # default
    tag: 'main'  # default
    comment: 'replace with specific tag or commit'  # default

```

## Inputs

### output_file

Output file name (default READMD.md).

Default: README.md

### commit_and_push

Push back changes made to Github.

Default: true

### tag

Tag or branch to use in example

Default: main

### comment

Comment after tag or branch to use in example

Default: replace with specific tag or commit

## Outputs

### changes_detected

Boolean if there were changes committed. Will be none if 'commit_and_push' was false.

### commit_hash

Commit hash if new data has been committed. Will be none if 'commit_and_push' was false.

