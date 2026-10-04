---
name: boomi-execute-and-query
description: Execute a Boomi process and then retrieve its execution records.
api: openapi/boomi-execution-api-openapi.yml
operations:
- executeProcess
- queryExecutionRecords
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/boomi-execution-api-openapi.yml ; every operationId checked against the contract
---

# boomi-execute-and-query

Execute a Boomi process and then retrieve its execution records.

## Steps

1. 1. Call `executeProcess` with the required request body (no specific fields or headers are documented).
2. 2. Call `queryExecutionRecords` with the query payload to fetch execution records (no specific fields or headers are documented).

## Rules

- Authentication: use either `basicAuth` or `bearerAuth` HTTP authentication schemes.
- Rate limiting: no rate limit is defined; on exhaustion the response is HTTP None.
