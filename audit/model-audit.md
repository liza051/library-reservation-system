
# Model Audit — Library Reservation System

## 1. Audit Purpose

The purpose of this audit is to compare the conceptual ER model with the system specification and identify inconsistencies between them.

## 2. Identified Discrepancies

### Discrepancy 1: Reader Phone Attribute

**Problem:**
The specification described the Reader phone number, while the initial ER model used the attribute `phone`.

**AI feedback:**
The attribute name should be consistent in the specification and the ER model.

**Correction:**
The attribute was standardized as `phone_number` in both files.

### Discrepancy 2: BookCopy Status Attribute

**Problem:**
The specification described the copy status, while the initial ER model used the generic attribute name `status`.

**AI feedback:**
The attribute should clearly identify that it represents the status of a physical book copy.

**Correction:**
The attribute was renamed to `copy_status` in the ER model and specification.

### Discrepancy 3: Book and BookCopy Cardinality

**Problem:**
The initial ER model required every Book to have at least one BookCopy, while the specification did not explicitly require this.

**AI feedback:**
The minimum number of physical copies should be clarified in the requirements.

**Decision:**
A Book can exist in the library catalog without physical copies.

**Correction:**
The specification was updated to allow zero or many BookCopies for one Book. The ER relationship was changed to:

`BOOK ||--o{ BOOK_COPY`

## 3. Verification Results

- The Reader phone attribute is consistent.
- The BookCopy status attribute is consistent.
- The Book–BookCopy cardinality matches the updated specification.
- The model contains eight entities.
- The model contains eight relationships.
- Reservation and Loan remain separate entities.
- The business rules for active loans are documented in the specification.

## 4. Conclusion

The identified inconsistencies were reviewed and corrected by clarifying the specification and aligning the ER model with the updated requirements.

Further verification of normalization and business rules is required.
