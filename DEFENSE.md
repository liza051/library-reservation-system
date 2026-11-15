# Project Defense — Library Reservation System

## 1. Project Intent

The Library Reservation System is designed to manage readers, books, physical book copies, reservations, loans, and returns in a library.

The purpose of this project is to create a conceptual Entity-Relationship (ER) model that describes the main entities, their attributes, relationships, and cardinalities.

## 2. Main Entities

The conceptual model contains eight entities:

- Reader
- Author
- Category
- Book
- BookCopy
- Reservation
- Loan
- Librarian

## 3. Main Relationships

- One Author can be associated with many Books.
- One Category can contain many Books.
- One Book can have many physical BookCopies.
- One Reader can create many Reservations.
- One BookCopy can be reserved many times over time.
- One Reader can have many Loans over time.
- One BookCopy can participate in many Loans over time.
- One Librarian can process many Loans.

## 4. Business Rules

- Each Book has exactly one Author and one Category.
- Reservations refer to individual physical copies.
- A Reader can have multiple active Reservations.
- A Reader can have only one active Loan at a time.
- A BookCopy can have only one active Loan at a time.
- Reservation and Loan are separate processes.
- A Loan stores issue date, due date, return date, and status.

## 5. Model Verification

The ER model is described using Mermaid ER Diagram syntax in `model/er-model.mmd`.

![Library Reservation System ER Diagram](model/er-model.svg)

The model must be checked against `spec.md` to ensure that all entities, attributes, relationships, and cardinalities are consistent.

## 6. Project Documentation

- `README.md` — project overview.
- `spec.md` — system requirements and acceptance criteria.
- `model/` — conceptual ER model and diagram.
- `adr/` — architectural decision records.
- `audit/` — model consistency audit.
- `ai/` — AI prompts, responses, and feedback.
- `DEFENSE.md` — project defense and verification results.

## 7. Scope

This project focuses on conceptual data modeling and requirements analysis. It does not include physical database implementation, SQL scripts, or application development.