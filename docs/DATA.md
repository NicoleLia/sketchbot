# Research data and anonymization

## Included materials

- `reference-images/` contains the four reference answers used in the criteria-and-reference condition.
- `model-evaluations/` contains checked-in JSONL, CSV, and summary outputs for Qwen3-VL 7B/32B under full and simple prompting conditions.
- `expert-ratings/ratings.csv` contains 1,360 anonymized ratings: four reviewers rated 340 feedback responses for diagnostic accuracy and guidance quality.

## Anonymization

The published rating table removes `participant`, `createdAt`, and `updatedAt`. It replaces reviewer identity with deterministic `reviewer_01` through `reviewer_04` identifiers. No mapping from these identifiers to people is included.

Aggregate files under `expert-ratings/aggregates/` contain only non-identifying study summaries. Files that retained reviewer identities, timestamps, notebook checkpoints, or editable review sessions are deliberately excluded.

## Reproduction limits

The VLM model weights, GPU hardware, model-serving environment, and API credentials are not bundled. Re-running a model can produce different outputs even with matching prompts. The supplied materials therefore support inspection of study inputs and results, and re-execution of the pipeline when a compatible model environment is available.
