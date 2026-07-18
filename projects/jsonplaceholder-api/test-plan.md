# Test Plan — JSONPlaceholder REST API

**Plan ID:** JP-TP-001  
**Author:** Alexander Lebedinskii  
**Date:** 18 July 2026

## Objective

Verify REST resource availability, response schemas, relationships, query filters, error handling and documented write-operation behavior.

## Scope and approach

GET coverage for posts, comments, users and todos; positive and negative IDs; query parameters; JSON schema and content-type checks. POST/PATCH/DELETE are included as non-persistent contract tests because the service documents that writes are simulated.

## Acceptance criteria

- Documented resources return JSON with the expected core fields.
- Existing IDs return the expected entity.
- Missing IDs do not return another user's data.
- Filters restrict results to the requested relationship.
- No server-side 5xx response is accepted for ordinary test data.

## Risks

This is a shared public fake API. Data is static and write operations do not persist, so persistence assertions are out of scope.

