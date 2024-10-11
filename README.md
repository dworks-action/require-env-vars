# Check Env Vars GitHub Action

This GitHub Action checks if certain environment variables are set and aborts execution early if any are missing.

## Usage

To use this action, include it in your workflow YAML file:

```yaml
name: Check Environment Variables

on: [push, pull_request]

jobs:
  examplpe:
  runs-on: ubuntu-latest
  steps:
    - name: Check Env Vars
      uses: dworks-action/require-env-vars@v0
      with:
        vars: VAR1 VAR2 VAR3
```

## Inputs

- `vars`: A space-separated list of environment variables to check.


## License

This project is licensed under the MIT License.