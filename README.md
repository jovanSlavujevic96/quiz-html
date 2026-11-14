# Claude Certified Developer – Foundations Practice Quiz

A lightweight, offline, local-browser quiz app. No installation, server, Node.js, Python runtime, or internet connection is required.

## Run
1. Extract the ZIP (if using the ZIP).
2. Double-click `index.html` to open it in Chrome, Edge, or Firefox.
3. The 53-question original practice bank is built into the app. Click **Use included question bank** and then **Start quiz**.
4. You can also load a separate compatible `.json` file using **Load JSON file**.

## Modes
- **Exam simulation:** 53 questions, 120-minute countdown, no explanations until submission.
- **Practice:** immediate feedback after checking each answer.
- **Quick practice:** 15 randomly selected questions.

Supports single-answer and multiple-answer questions, exact selection limits, question navigation, flags, scoring, domain breakdown, retrying incorrect/unanswered questions, and exporting results.

## Question-bank JSON format
The app accepts either a top-level array or an object with a `questions` array.

```json
{
  "questions": [
    {
      "id": 1,
      "domain": "Tools & MCP",
      "type": "multiple",
      "question": "Which TWO statements are correct?",
      "select": 2,
      "options": [
        {"id": "A", "text": "First option"},
        {"id": "B", "text": "Second option"},
        {"id": "C", "text": "Third option"}
      ],
      "correct": ["A", "C"],
      "explanation": "Why A and C are correct."
    }
  ]
}
```

For a single-answer question, use `"type": "single"` and one item in `correct`. For multiple-answer questions, use `"type": "multiple"`, set `select` to the exact number required, and provide that many IDs in `correct`.

## Important notes
- The included questions are original practice questions written for study. They are **not** official Anthropic exam questions and do not reproduce a confidential live question bank.
- The practice score is a raw percentage, not an official scaled score or a prediction of passing.
- The app is a study aid. It does not guarantee that every topic or detail matches the current exam version. Check the current official candidate guide for exam logistics and objectives.
- This is intentionally a local convenience app, not a secure test environment. The answer key is present in the local HTML source and JSON bank; do not use it to administer a high-stakes exam.
- No answers or personal data are transmitted anywhere. Exported results are saved only when you choose to download them.
