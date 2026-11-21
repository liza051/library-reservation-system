# AI Work Log — Library Reservation System

## 1. Purpose of AI Assistance

AI was used as a supporting tool during the development of the Library Reservation System conceptual ER model.

Its role was to assist with requirements analysis, identify possible gaps and inconsistencies, ask clarifying questions, and suggest alternative solutions.

## 2. AI-Assisted Analysis

### Task 1: Specification Review

**User input:**

The project specification describing readers, authors, categories, books, physical copies, reservations, loans, and librarians was provided for analysis.

**AI contribution:**

AI helped review the entities, attributes, relationships, and business rules. It identified potentially unclear requirements and suggested possible clarifications.

**My decisions:**

I reviewed the suggestions and retained the original eight entities and the rule that each Book has exactly one Author.

### Task 2: ER Model Review

**User input:**

The Mermaid ER model was compared with the project specification.

**AI contribution:**

AI helped identify differences in attribute names and the Book–BookCopy cardinality and suggested possible ways to resolve them.

**My decisions:**

I reviewed the identified differences and standardized the attribute names as `phone_number` and `copy_status`.

I also clarified that a Book can exist in the catalog without physical copies.

### Task 3: Audit Preparation

**User input:**

The updated specification and ER model were checked for consistency.

**AI contribution:**

AI helped identify possible discrepancies between the specification and the model, asked clarifying questions, and suggested ways to document the corrections.

**My decisions:**

I evaluated the suggestions and selected the corrections that matched the project requirements. I included the final decisions in the project documentation.

## 3. Review of AI Suggestions

AI suggestions were treated as recommendations and were not accepted automatically.

The project requirements and modeling decisions were reviewed by the student. The final decisions about the number of authors per book and the possibility of books existing without physical copies were made by the student and reflected in the specification.

## 4. Conclusion

AI was used as an analytical assistant for requirements review, identification of gaps, clarification of relationships, and consistency checking.

The student independently evaluated the suggestions and made the final modeling decisions. Responsibility for the completed ER model and its documentation remains with the student.

## 5. AI Documentation Files

The reconstructed prompts, summarized AI responses, and personal feedback are stored separately:

- `ai/prompts/01-specification-review.md`
- `ai/prompts/02-er-model-review.md`
- `ai/responses/01-specification-review-response.md`
- `ai/responses/02-er-model-review-response.md`
- `ai/feedback.md`

The prompts and responses are reconstructed summaries of the project work, not verbatim conversation transcripts.

The feedback document records which AI recommendations were accepted and explains the final modeling decisions.