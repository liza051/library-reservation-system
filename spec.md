# Specification — Library Reservation System

## 1. System Intent

The Library Reservation System manages library readers, books, physical book copies, reservations, loans, and book returns. The system is designed to track individual physical copies and the interactions between readers and library staff.

## 2. Entities and Attributes

- **Reader** — full name, email, phone_number, registration date.
- **Author** — full name.
- **Category** — name and description.
- **Book** — title, ISBN, publication year.
- **BookCopy** — inventory number, copy_status, location.
- **Reservation** — reservation date, expiration date, status.
- **Loan** — issue date, due date, return date, status.
- **Librarian** — employee's full name, email.

## 3. Relationships and Business Rules

- One Author can be associated with many Books; each Book has exactly one Author.
- One Category can contain many Books; each Book belongs to exactly one Category.
- One Book can have zero or many BookCopies; each BookCopy belongs to exactly one Book.
- One Reader can create many Reservations; each Reservation belongs to exactly one Reader.
- One BookCopy can have many Reservations over time; each Reservation concerns exactly one BookCopy.
- One Reader can have many Loans over time, but only one active Loan at a time.
- One BookCopy can have many Loans over time, but only one active Loan at a time.
- One Librarian can process many Loans; each Loan is processed by one Librarian.
- A Reservation and a Loan are separate processes.
- A Loan stores its status and return date. The return date is recorded when the book is returned.
- A Reader can have multiple active Reservations simultaneously.
- An active Loan represents a book that has not yet been returned.

## 4. Acceptance Criteria

- Every Book has exactly one Author and one Category.
- Every BookCopy belongs to exactly one Book.
- A Book can exist in the catalog without physical copies.
- Reservations refer to individual physical copies, not just book titles.
- A Reader can have multiple active Reservations.
- A Reader cannot have more than one active Loan.
- A BookCopy cannot have more than one active Loan.
- A Loan records its issue date, due date, return date, and status.
- The return date is recorded when a Loan is completed.
- Each Loan is associated with one Librarian.
- Reservation and Loan are represented as separate entities.
- The conceptual model is reviewed for normalization to at least 3NF.
- All entity relationships and cardinalities are consistent with these requirements.