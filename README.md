[![YAML Validator](https://github.com/cedadev/collection-descriptions/actions/workflows/tests.yaml/badge.svg)](https://github.com/cedadev/collecion-descriptions/actions/workflows/tests.yaml)

# Collection Descriptions

These documents are to describe how to process the files within a dataset and extract facets.
These documents are aggregated along the branch with the information lower in the tree taking 
precendence. See [example](example/full_example.yml) file or [documentation](https://cedadev.github.io/stac-generator/collection_descriptions/collection_descriptions.html)
for more details.

## Validation

The collection-descriptions are validated against https://github.com/cedadev/collection_description_validator.

If you wish to check your files before committing, there are two options:
1. Create a python environment and run it manually
2. Install the validation as a pre-commit hook to always check when you try to commit

### Python env

1. `python -m venv venv`
2. `. venv/bin/activate`
3. `pip install git+https://github.com/cedadev/collection_description_validator`
4. `collection-desc-validator descriptions/`

### Pre-commit hook
The hook automates testing on your own machine

1. `pip install pre-commit`
2. `pre-commit install`

**NOTE: You could use a python virtual environment for this if you wanted**

You are done, the hook will run when you make a commit.
