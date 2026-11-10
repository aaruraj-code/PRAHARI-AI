# Safe synthetic test cases

These are invented examples for demonstrating warning indicators. The `.example.test` domain is reserved for testing and is not a real bank or service.

| ID | Input | Expected demo behaviour |
|---|---|---|
| T1 | Your bank account will be blocked today. Verify immediately at http://secure-bank-login.example.test | High: urgency + verification language + HTTP/test domain |
| T2 | Congratulations! You won a free prize. Pay a small processing fee now to claim it. | Medium/High: prize + fee + claim language |
| T3 | Please review the attached invoice urgently. I was not expecting an invoice from this sender. | Medium: urgency; user should independently verify sender |
| T4 | Hi, our study group meeting is at 4 pm in the library. Please bring your notebook. | Low: no obvious warning pattern |
| T5 | http://paypal-account-verify.example.test/login | Medium/High depending on URL rules: HTTP + suspicious wording + reserved test domain |

## How to evaluate
1. Run each sample through the demo.
2. Record the displayed category and explanation.
3. Note whether the result is sensible.
4. Add benign examples that contain words like “urgent” to observe false positives.
5. Add suspicious examples with no obvious trigger words to observe false negatives.

Do not report an accuracy percentage from these few hand-picked examples. A meaningful accuracy evaluation needs a larger, labelled dataset and a separate test set.
