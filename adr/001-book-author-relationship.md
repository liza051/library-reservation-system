
# ADR 001: One Author per Book

## Status

Accepted

## Context

The Library Reservation System requires a relationship between books and authors.

During the conceptual data modeling process, it was necessary to decide whether one book could have multiple authors or exactly one author.

## Decision

Each Book is associated with exactly one Author.

One Author can be associated with zero or many Books.

The ER relationship is:

`AUTHOR ||--o{ BOOK : writes`

## Alternatives Considered

1. One Book has exactly one Author.
2. One Book can have multiple Authors.

## Consequences

- The conceptual model remains simple.
- Every Book must have one Author.
- One Author can write multiple Books.
- A many-to-many relationship between Book and Author is not required.

## Rationale

The first option was selected to follow the project specification and keep the model consistent with the chosen business requirements.
