
# AI Work Log — Library Reservation System

## 1. Purpose of AI Usage

AI was used to review the requirements and conceptual ER model of the Library Reservation System, identify inconsistencies, and suggest possible corrections.

## 2. AI-Assisted Work

### Task 1: Specification Review

**User input:**
The project specification describing readers, authors, categories, books, physical copies, reservations, loans, and librarians was provided for review.

**AI contribution:**
AI reviewed the entities, attributes, relationships, and business rules and suggested clarifications.

**My decision:**
I kept the original eight entities and the rule that each Book has exactly one Author.

### Task 2: ER Model Review

**User input:**
The Mermaid ER model was provided for comparison with the specification.

**AI contribution:**
AI identified differences in attribute names and the Book–BookCopy cardinality.

**My decision:**
I standardized the attribute names as `phone_number` and `copy_status`.

I also clarified that a Book can exist in the catalog without physical copies.

### Task 3: Audit Preparation

**User input:**
The updated specification and ER model were reviewed for consistency.

**AI contribution:**
AI helped organize the identified discrepancies and document their corrections.

**My decision:**
I reviewed the proposed changes and included the corrections in the project documentation.

## 3. AI Output Review

The AI suggestions were not accepted automatically.

The project decisions were checked against the system requirements. The final decisions about the number of authors per book and the existence of books without physical copies were retained in the specification.

## 4. Conclusion

AI was used as an assistant for requirements analysis, ER model review, and documentation.

The final modeling decisions were reviewed and approved by the project author.

## 5. AI Documentation Files

The reconstructed prompts, summarized AI responses, and personal feedback are stored separately:

- `ai/prompts/01-specification-review.md`
- `ai/prompts/02-er-model-review.md`
- `ai/responses/01-specification-review-response.md`
- `ai/responses/02-er-model-review-response.md`
- `ai/feedback.md`

The prompts and responses are reconstructed summaries of the project work, not verbatim conversation transcripts.

The feedback document records which AI recommendations were accepted and explains the final modeling decisions.