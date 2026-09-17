# Python Diagnostic and Daily Practice

Prepared: 17 September 2026. Starting level: basic Python. Goal: write, explain, debug, and test small programs that support later ML/CV work.

## Daily routine

The requested reminder is scheduled for 12:00 noon in the current local timezone, Asia/Shanghai (UTC+8). Spend 20 minutes, optionally extending to 30. On busy days do 10 minutes of review. Weekend practice counts within the weekend coding allocation. The reminder checks reported progress before raising difficulty; it must not assume completion.

First read and restate the task. Work independently; Python syntax documentation is allowed. After 15–20 minutes stuck, request one hint rather than a full solution. Keep the unsuccessful attempt because it identifies the next learning need. Provide code, time spent, hint use, tests, and a short explanation for feedback. No solution is included in this document.

## Initial diagnostic: three short sessions

1. **[LeetCode 1480 — Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/)**, up to 20 minutes. Use a plain loop for the first attempt. Explain how the accumulated value changes. Test a single value and a list containing negative numbers. State whether the input list is changed. This instructional loop restriction is ours, not a requirement stated by LeetCode.
2. **[LeetCode 217 — Contains Duplicate](https://leetcode.com/problems/contains-duplicate/)**, up to 20 minutes. Find a correct solution first. Then explain whether a set or dictionary would help. Test unique values, repeated values, and negative values. Keep both initial and improved attempts if you make a change.
3. **Math-to-Python bridge**, up to 20 minutes. Write a function that takes a nonempty list of numbers and returns its arithmetic mean and population variance. Use denominator n, not n−1. State how an empty input should be handled. Hand-check [1, 2, 3], a single number, and repeated identical values. NumPy is not needed for the first version.

Spread the diagnostic over separate days if needed. It is a skills check, not a timed competition. A partial solution is useful evidence.

## First seven practice sessions

| Session | Task | Focus |
|---|---|---|
| 1 | Diagnostic 1: Running Sum | Loops, indexing, accumulation, explaining state |
| 2 | Re-solve Running Sum without looking; add edge-case tests | Recall, debugging, input mutation |
| 3 | Diagnostic 2: Contains Duplicate | Lists, sets, membership, reasoning about repeated work |
| 4 | Diagnostic 3: arithmetic mean and population variance | Functions, numerical reasoning, maths-to-code |
| 5 | [LeetCode 1 — Two Sum](https://leetcode.com/problems/two-sum/) as an optional stretch | Try a correct pair-search first; discuss a dictionary only after understanding it. If earlier tasks were hard, review them instead. |
| 6 | Write a dot-product function for equal-length lists | Loop version first; compare with NumPy when ready; define behavior for unequal lengths |
| 7 | Explain and re-solve the weakest exercise; write a short log | Retention and communication; no new problem required |

These are proposed sessions, not completed work. Future exercises depend on submitted attempts. Revisit difficult problems after two days and one week inside existing review slots.

## Feedback rubric

For each dimension, record 0 (not yet), 1 (with support), or 2 (independent):

- Correctness: meets the stated contract and passes appropriate examples.
- Reasoning: can explain each step and important variables.
- Tests: covers relevant boundary cases and can explain expected results.
- Python clarity: sensible names, functions, and appropriate basic data structures.
- Complexity: can describe how time and memory change with input size; initially informal reasoning is sufficient.

Use the profile to choose the next exercise rather than ranking yourself by total score. Difficulty increases only when recent easy tasks can be solved and explained again without a copied solution. During the first week, correctness and explanation matter more than speed or advanced optimization.

## Longer-term progression

- Weeks 1–2: loops, lists, strings, functions, simple tests, reading tracebacks.
- Weeks 3–4: dictionaries, sets, counting, sorting, simple complexity reasoning.
- Weeks 5–8: two pointers and simple binary search when ready; mathematical functions, matrix shapes, NumPy indexing and broadcasting.
- Later: maintain basic problem-solving while shifting more exercises toward data loading, numerical calculations, plotting, model evaluation, and image arrays.

Use three small new problems, two review/debugging sessions, one maths/NumPy bridge, and one weekly explanation as the default pattern. Avoid turning LeetCode into a separate large course competing with maths, IELTS, and university work.

## Submission template

- Problem and link:
- Date and time spent:
- My understanding of the task:
- My code:
- Examples I tested and their results:
- Hints or tools I used:
- Time/space complexity, if I can explain it:
- What I am unsure about:

## First assignment

Start with Running Sum. Return your code and explain what happens on the input [3, -1, 4, 2]. Describe the expected output before running it. Try the loop yourself before requesting help; a partial attempt is welcome.
