# AI Prompt 01 — Specification Review

## Purpose

Review the initial specification of the Library Reservation System.

## Reconstructed Prompt
This prompt is reconstructed from the project work and is not a verbatim transcript of the original conversation.

Analyze the specification of a Library Reservation System.

The system includes the following entities:

- Reader
- Author
- Category
- Book
- BookCopy
- Reservation
- Loan
- Librarian

Check whether the entities, attributes, relationships, cardinalities, and business rules are clear and consistent.

Pay special attention to:
- The relationship between Book and Author.
- The relationship between Book and BookCopy.
- Reservations of individual physical copies.
- Active loans and book returns.
- The separation between Reservation and Loan.

Identify possible ambiguities and suggest corrections. Do not change the requirement that each Book has exactly one Author.

## My Feedback

I reviewed the suggestions and decided to keep exactly one Author for each Book. I also clarified that a Book may exist in the catalog without physical copies.