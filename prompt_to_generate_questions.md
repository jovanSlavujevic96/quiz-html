# The exam is "Claude Certified Developer - Foundations"

Generate questions for the exam.
Example question structure:
```JSON
{
  "id": 1,
  "domain": "Applications & Integration",
  "type": "multiple",
  "question": "Which statements about prompt caching are correct?",
  "select": 2,
  "options": [
    {"id": "A", "text": "Option A"},
    {"id": "B", "text": "Option B"},
    {"id": "C", "text": "Option C"},
    {"id": "D", "text": "Option D"}
  ],
  "correct": ["A", "C"],
  "explanation": "Explanation of the correct answers."
}
```

## Bad example of questions:

Some of the questions were too easy. For example:
- "Where should you store an API key?" — fairly straightforward.
- "What is prompt injection?" — basic terminology.
- "What is MCP designed to provide?" — basic definition.

Some distractors were also too obviously incorrect.
For example, choosing between:
- Use bounded concurrency.
- Launch unlimited parallel requests.
- Disable timeouts.

Generate me Advanced mock examination
53 questions, significantly harder scenarios, plausible distractors and more detailed technical questions.
