# AI Feedback — Library Reservation System

## Feedback 01 — Specification Review

The AI recommendations helped clarify the system requirements.

I agreed that the Book and BookCopy entities should remain separate because the system manages individual physical copies.

I decided to keep exactly one Author for each Book, as required by my chosen project scope.

I also clarified that a Book may exist in the catalog without physical copies.

## Feedback 02 — ER Model Review

The AI identified three inconsistencies between the initial specification and the ER model:

1. The Reader phone attribute had inconsistent names.
2. The BookCopy status attribute had inconsistent names.
3. The minimum cardinality between Book and BookCopy was not clearly defined.

I accepted these findings and updated the specification and ER model.

I also confirmed that the restriction of one active Loan per Reader and per BookCopy is a business rule that requires additional documentation beyond basic ER cardinalities.

## Final Evaluation

I did not accept AI suggestions automatically. I reviewed them against the project requirements and made the final modeling decisions myself.