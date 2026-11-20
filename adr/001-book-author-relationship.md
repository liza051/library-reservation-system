# ADR 001: One Author per Book

## Status

Accepted

## Context and Problem Statement

The Library Reservation System requires a relationship between books and authors. A modeling decision is needed to define whether a book can have one author or multiple authors.

## Decision Drivers

- Consistency with the project specification.
- Simplicity of the conceptual ER model.
- Clear relationship cardinalities.
- Compliance with the selected project scope.

## Considered Options

1. Each Book has exactly one Author.
2. A Book can have multiple Authors.

## Decision Outcome

Chosen option: **Each Book has exactly one Author.**

One Author can be associated with zero or many Books.

The ER relationship is:

`AUTHOR ||--o{ BOOK : writes`

## Consequences

- Every Book must be associated with exactly one Author.
- One Author can be associated with multiple Books.
- A many-to-many relationship is not required.
- The model remains consistent with the selected specification.

## Confirmation

The decision is reflected in `spec.md` and `model/er-model.mmd` and is documented in the project defense.
