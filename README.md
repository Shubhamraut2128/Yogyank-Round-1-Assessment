# Yogyank Round 1 Assessment

## Objective

Audit and improve the baseline entitlement score training pipeline.

## Fixes Implemented

- Removed future leakage feature
- Removed policy manipulation from target
- Replaced LabelEncoder with OneHotEncoder
- Added deterministic validation
- Added sklearn pipeline
- Added artifact saving
- Added schema and metadata saving
- Added reason-code generation

## Validation Strategy

Used deterministic holdout split without shuffle.

## Artifacts

- yogyank_pipeline.pkl
- schema.json
- version.json

## Run Command

python fixed_yogyank_training.py

## Limitations

- Synthetic dataset
- No production monitoring
- No drift detection

"""

with open("README.md", "w") as f:
    f.write(readme)

print("README.md created")
