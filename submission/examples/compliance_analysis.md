# Compliance Analysis: submission.yaml vs 5_3_schema.json

## 1. Keys in submission.yaml NOT compliant with the schema:

**No non-compliant keys found** - all keys in submission.yaml are valid according to the schema.

## 2. Keys available in schema but NOT present in submission.yaml:

### Checkout section - Missing optional fields:
- `_timestamp`
- `git_commit_name`
- `git_commit_tags`
- `git_commit_message`
- `git_repository_branch`
- `git_repository_branch_tip`
- `patchset_files`
- `patchset_hash`
- `message_id`
- `comment`
- `start_time`
- `origin_builds_finish_time`
- `origin_tests_finish_time`
- `log_url`
- `log_excerpt`
- `misc`

### Build section - Missing optional fields:
- `_timestamp`
- `comment`
- `duration`
- `command`
- `compiler`
- `input_files`
- `output_files`
- `config_name`
- `config_url`
- `log_url`
- `log_excerpt`
- `misc`

### Test section - Missing optional fields:
- `_timestamp`
- `environment`
- `comment`
- `log_url`
- `log_excerpt`
- `number`
- `duration`
- `input_files`
- `output_files`
- `misc`

### Issue section - Missing optional fields:
- `_timestamp`
- `comment`
- `misc`

### Incident section - Missing optional fields:
- `_timestamp`
- `comment`
- `misc`

### Root level - Missing optional field:
- `minor` (in version object - only `major` is required)

## Summary

All missing fields are **optional** according to the schema. The submission.yaml file contains all required fields and is fully compliant with the 5_3_schema.json specification.
