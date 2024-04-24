# create-ecr-repo-action

Github Action to create an ECR repository if it's missing.

## Inputs

### `environment`
[**Required**] Finalcad envrionment: production, staging, sandbox

### `registry`
[**Required**] Full registry name

### `pulling-accounts`
Comma separated list of account number allowed to pull beside principal account, Default: empty

### `retention-number`
Number of images to keep, Default: 5

## Usage

```yaml
- name: Create ecr
  uses: e-berger/create-ecr-repo-action@v1
  with:
    registry: api-service-test
```
