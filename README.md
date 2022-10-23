# Auto-Action-Readme


Version: 0.1.0





Github Action to use the settings in action.yml to populate the readme.


## Usage

```yaml

- uses: ajparsons/auto-action-readme@36b4d640bbefc7449cc9d2b36842fa5b8e712f0b
# If you trust this source, use ajparsons/auto-action-readme@v0
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


