# Auto-Action-Readme

Version: 1.0.0

Github Action to use the settings in action.yml to populate the readme.

## Usage

```yaml

# It is better practice to use the SHA hash of this tag rather than the tag itself.
- uses: ajparsons/auto-action-readme@v1
  id: example-step 
  with:
    output_file: 'README.md'  # default
    commit_and_push: 'true'  # default
    tag: 'main'  # default

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

## Outputs

### changes_detected

Boolean if there were changes committed. Will be none if 'commit_and_push' was false.

