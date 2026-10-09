---
name: boomi-create-repository
description: Create a new repository, retrieve its details, and list all repositories.
api: openapi/boomi-repositories-api-openapi.yml
operations:
- createRepository
- getRepository
- listRepositories
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/boomi-repositories-api-openapi.yml ; every operationId checked against the contract
---

# boomi-create-repository

Create a new repository, retrieve its details, and list all repositories.

## Steps

1. 1. `createRepository` – send a POST request with the repository fields in the request body (as defined in the contract).
2. 2. `getRepository` – send a GET request with the `repositoryId` path parameter returned from the create step.
3. 3. `listRepositories` – send a GET request to retrieve the collection of repositories.

## Rules

- Authentication: include either a Basic Auth header or a Bearer token as defined by the `basicAuth` or `bearerAuth` schemes.
- Idempotency: the `createRepository` operation is not idempotent; repeat calls may create duplicate repositories.
