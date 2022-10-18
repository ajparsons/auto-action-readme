# Auto-Action-Readme


Version: 0.1.0





Github Action to use the default in action.yml to populate the readme.


## Usage

```yaml

- uses: ajparsons/auto-action-readme@v0.1.0
    id: example-step 
    with:
        output_file: 'README.md' 
        commit_and_push: 'true' 

```


## Inputs

### output_file

Output file name (default READMD.md)
Default: README.md



### commit_and_push

Push back inside this action (default true)
Default: true





## Outputs

### changes_detected

Boolean on if there were changes committed


