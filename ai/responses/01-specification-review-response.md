# AI Response 01 — Specification Review

## Reconstructed AI Response

The specification describes the main entities required for a Library Reservation System. The separation between Book and BookCopy is appropriate because one book title may have multiple physical copies.

The relationship between Book and Author should follow the selected business rule: each Book has exactly one Author, while one Author may be associated with multiple Books.

Reservations should refer to individual physical copies rather than only book titles. Reservation and Loan should remain separate entities because reserving a copy and borrowing it are different processes.

The specification should also clarify that:
- A Book may exist in the catalog without physical copies.
- A Reader may have multiple active Reservations.
- A Reader may have only one active Loan at a time.
- A BookCopy may have only one active Loan at a time.
- The return date is recorded when a Loan is completed.

## My Evaluation

I accepted the recommendations about clarifying the Book–BookCopy relationship and keeping Reservation and Loan separate.

I retained the decision that each Book has exactly one Author.

This response is reconstructed as a summary of the AI-assisted analysis, not a verbatim transcript.