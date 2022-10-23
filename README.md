# Auto-Action-Readme


Version: 0.1.0





Github Action to use the settings in action.yml to populate the readme.


## Usage

```yaml

- uses: ajparsons/auto-action-readme@8f4153e9891533f6fef20b5a5a34f21ae37d4174 # If you trust this source, use @v0
  id: example-step 
  with:
    output_file: 'README.md'  # default value
    commit_and_push: 'true'  # default value
    tag: 'main'  # default value

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


