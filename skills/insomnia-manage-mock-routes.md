---
name: insomnia-manage-mock-routes
description: Create, view, update, and delete mock routes for a mock server.
api: openapi/insomnia-mock-routes-api-openapi.yml
operations:
- listMockRoutes
- createMockRoute
- updateMockRoute
- deleteMockRoute
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/insomnia-mock-routes-api-openapi.yml ; every operationId checked against the contract
---

# insomnia-manage-mock-routes

Create, view, update, and delete mock routes for a mock server.

## Steps

1. 1. Use `listMockRoutes` – requires `Authorization: Bearer <token>` header.
2. 2. Use `createMockRoute` – requires `Authorization: Bearer <token>` header and the request body fields defined for a mock route.
3. 3. Use `updateMockRoute` – requires `Authorization: Bearer <token>` header, path parameters `mockServerId` and `routeId`, and the request body fields for updating a mock route.
4. 4. Use `deleteMockRoute` – requires `Authorization: Bearer <token>` header and path parameters `mockServerId` and `routeId`.

## Rules

- Authentication: Include `Authorization: Bearer <token>` header for all operations.
- No rate limiting is defined; exhaustion returns no specific HTTP status.
- Pagination: Not applicable to these endpoints.
- Errors: Follow standard HTTP error responses as defined by the API.
