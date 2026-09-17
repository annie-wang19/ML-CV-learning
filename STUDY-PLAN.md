# Weekend Plan: Machine Learning, Computer Vision, and English

Prepared: 17 September 2026.

## Starting point

You are a third-year undergraduate with basic Python and coursework in advanced mathematics, linear algebra, probability, numerical computation, computer algorithms, error theory, and measurement adjustment. You explicitly report that your mathematical foundations for ML are weak. Prior course exposure must not be treated as current mastery. You scored 94 on TOEFL in summer 2025 without specific preparation. Your IELTS target is 7.5, with a tentative test date in the winter holiday around February 2027. Available weekly hours, current IELTS component levels, required component minimums, and IELTS test type remain to be confirmed.

My prospective supervisor recommends improving English and ML knowledge, programming and systematic AI-assisted coding, protecting university grades, Hung-yi Lee's introductory deep-learning material, and Daniel Cremers's Multiple View Geometry course. These recommendations specify no deadline or course edition. The schedule below is a proposal based on those recommendations.

Start with **eight hours per weekend: six technical hours and two English hours**, plus a proposed 20-minute English session and a 20-minute Python session on five weekdays. Weekend coding reminders point to the existing weekend coding block, so they do not add two more sessions. This provisional budget totals about 11 hours 20 minutes per week and must be reduced if university work requires it. Protect at least two technical hours for mathematics. Rebalance after an English diagnostic. Use 28 study weekends for the technical roadmap, approximately seven months before exam breaks; it extends beyond the February 2027 IELTS target. Do not compress weak mathematics to finish the technical roadmap before IELTS. During the final four to six weeks before IELTS, shift weekend time from six technical/two English hours to four technical/four English hours; extend the technical schedule accordingly. During university exams, pause new material and resume afterward without catch-up debt.

Treat mathematical understanding and Python implementation as two equally necessary foundations. Begin with a low-pressure diagnostic and rebuild weak topics explicitly. For each idea, connect an intuitive explanation, a short derivation, a hand-worked numerical example, and a NumPy implementation. Move on when you can explain why the calculation works, not merely when the code runs. The first eight weekends provide a foundation block; they are not a deadline for mastering mathematics.

## What to learn first

ML learns patterns from data. Deep learning is a subset of ML using multilayer neural networks. Computer vision studies images and video; it includes both learned recognition and geometric methods.

| Area | Initial scope | Ability to demonstrate |
|---|---|---|
| Python and tools | Functions, loops, lists/dictionaries, imports, files, tracebacks, NumPy, plotting, basic Git | Load data, inspect shapes, plot results, debug an error, and save a meaningful commit |
| Mathematical foundations | Vectors, matrix products, rank, least squares, derivatives, gradients, chain rule, probability, expectation/variance, likelihood; eigenvalues and SVD | Explain symbols and assumptions, derive a small result, calculate by hand, and check it in code |
| ML | Regression, classification, losses, gradient descent, train/validation/test splits, overfitting, regularization, metrics | Fit a simple baseline and explain its evaluation |
| Deep learning | Tensors, layers, activations, backpropagation, batches, learning rates, training/evaluation, CNNs | Train a small network and interpret learning curves and errors |
| Geometric CV | Coordinates, projection, feature matching, robust estimation, epipolar geometry, triangulation | Visualize how camera observations constrain 3D points |

Measurement adjustment can eventually offer a bridge: residuals, least squares, and linearization reappear in geometric estimation. Rebuild those concepts if they are not secure before using that connection. Later, bundle adjustment jointly refines camera parameters and 3D points. Neural-network training also minimizes an objective, although its models and optimization procedures differ.

## Core resources

Use two main courses and open supporting documentation only when needed.

- **[Hung-yi Lee: Machine Learning 2021](https://speech.ee.ntu.edu.tw/~hylee/ml/2021-spring.php).** A proposed edition because the recommendation does not specify one. The official page includes ML/DL foundations, regression, classification, CNN work, and PyTorch support. Initially select these topics and reduce assignment scope where necessary. The [2020 course page](https://speech.ee.ntu.edu.tw/~tlkagk/courses_ML20.html) provides clearly grouped regression, gradient-descent, classification, and backpropagation resources if additional explanation is needed.
- **[Daniel Cremers: Multiple View Geometry](https://cvg.cit.tum.de/teaching/online/mvg).** Focus first on Chapters 1–5: mathematical foundations through two-view reconstruction; preview optimization later. The official online page pairs 2013/14 recordings with mostly compatible 2019 slides and notes minor differences. Geometry does not require completing deep learning first.
- **[Python Tutorial](https://docs.python.org/3/tutorial/)** and **[NumPy beginner guide](https://numpy.org/doc/stable/user/absolute_beginners.html)**: selected reference material for exercises. The Python tutorial assumes some programming knowledge.
- **[PyTorch: Learn the Basics](https://docs.pytorch.org/tutorials/beginner/basics/intro.html)**: a practical neural-network workflow after Python and introductory DL concepts; includes FashionMNIST and local/Colab options.
- **[OpenCV camera calibration and 3D tutorials](https://docs.opencv.org/4.x/d9/db7/tutorial_py_table_of_contents_calib3d.html)**: practical support for geometric concepts.
- **[Official IELTS Academic sample questions](https://www.ielts.org/take-a-test/preparation-resources/sample-test-questions/academic-test)**: an initial diagnostic and task practice. Academic is provisional until the required test type is confirmed. Set your own timer for untimed online practice.

## Twenty-eight study weekends

These are introductory learning units, not a promise to finish both full university courses. Each output should be small enough to explain and rerun.

| Week | Main focus | Evidence to save |
|---|---|---|
| 1 | Diagnostic; vectors, dot products, norms; Python functions and arrays | Compute a dot product by hand and in NumPy; explain its meaning and dimensions; record English baseline |
| 2 | Matrices as transformations, multiplication, transpose, rank; NumPy indexing | Transform and plot 2D points; explain matrix multiplication versus elementwise multiplication |
| 3 | Functions, derivatives, partial derivatives; plotting | Derive a simple squared-error derivative and compare it with a finite difference |
| 4 | Gradients, chain rule, gradient descent | Differentiate a small composite function and visualize one optimization step |
| 5 | Random variables, expectation, variance, covariance, conditional probability | Calculate a tiny example by hand and compare with a simulation |
| 6 | Probability distributions, likelihood, logs; ML orientation | Explain likelihood using coin tosses and compute a log-likelihood; distinguish probability from likelihood |
| 7 | Least squares, projections; eigenvalue/SVD intuition | Fit noisy points with a numerical least-squares solver; explain residuals and inspect a small SVD reconstruction |
| 8 | Foundation review and catch-up; geometry orientation | Explain a simple loss gradient and least-squares fit independently; sketch camera projection; repeat weak topics |
| 9 | Regression, losses, optimization | Implement linear-regression gradient descent; compare with the least-squares solution |
| 10 | Classification, logistic regression, cross-entropy | Fit a small baseline; explain how likelihood relates to the classification loss |
| 11 | Generalization, regularization, splits, metrics | Show overfitting; compare train/validation performance; keep test data untouched during tuning |
| 12 | Review and catch-up | Re-run the baseline and explain its split, metric, and one failed experiment without notes |
| 13 | PyTorch tensors and autograd | Reproduce the regression example; compare automatic gradients with a hand calculation |
| 14 | Layers, activations, backpropagation | Apply the chain rule to a tiny network; train a small MLP and trace dimensions |
| 15 | Training loops, batches, learning rate, evaluation | Plot train/validation loss; diagnose one problem; explain gradient clearing and evaluation mode |
| 16 | Convolution, stride, padding, pooling | Calculate a tiny convolution by hand; trace CNN shapes and run a forward pass |
| 17 | Image-classification experiment | Train a small CNN on FashionMNIST; compare it with an MLP under the same split |
| 18 | Review, error analysis, reproducibility | Save actual measured metrics and misclassified examples; provide rerun instructions |
| 19 | Coordinate frames, rotation, translation; SVD reinforcement | Transform synthetic 3D points with an explicit coordinate convention |
| 20 | Projection, intrinsics/extrinsics, homogeneous coordinates | Project a synthetic scene into two cameras and label each matrix |
| 21 | Features and correspondence | Match points in an image pair and visualize mismatches |
| 22 | Outliers, RANSAC, planar homography | Estimate a transform for two views of a flat object; explain its assumptions |
| 23 | Epipolar geometry, fundamental/essential matrices | Draw epipolar lines and distinguish calibrated from uncalibrated coordinates |
| 24 | Triangulation with known synthetic cameras | Recover 3D points, reproject them, and measure error |
| 25 | Geometry experiment and failure analysis | Add noise/outliers and compare results; real-image pose recovery is optional |
| 26 | Consolidation and bundle-adjustment intuition | Explain camera/point refinement and the least-squares objective; no full solver required |
| 27 | Project polish and catch-up | Make classifier and geometry examples easy to run; document assumptions and limitations |
| 28 | Review and communication | Give a five-minute English explanation and prepare a one-page progress report |

Start geometry earlier if the supervisor prioritizes it and the foundations are comfortable. Move existing hours to it rather than increasing the workload. Keep transformers, diffusion models, NeRF, Gaussian splatting, and complete SLAM systems as later topics unless a specific research need changes the priorities.

## Progress checks

- After Week 4: explain dot products, matrix dimensions, a derivative, and a simple chain-rule calculation. Repeat any weak unit.
- After Week 8: explain a simple gradient and least-squares fit, compute expectation/variance on a tiny example, and translate them into Python. Add foundation weekends when needed.
- After Week 12: explain baseline, loss, split, and overfitting. Repeat a smaller exercise if necessary.
- After Week 18: run the classifier, explain its training loop and backpropagation on a tiny example, and investigate errors. High accuracy by itself is insufficient.
- After Week 26: explain projection, matching, and triangulation using a working visualization. Synthetic data is sufficient.
- After Week 28: present two reproducible small projects and clearly state remaining gaps.

## A normal weekend

| Session | Time | Activity |
|---|---|---|
| Saturday | 120 minutes | Mathematics: intuition, derivation, hand calculation, and a short check |
| Saturday | 60 minutes | One Python/ML/CV concept or lecture segment |
| Saturday | 60 minutes | IELTS listening/reading task and error review |
| Sunday | 120 minutes | Build/debug one experiment and compare results |
| Sunday | 60 minutes | Explain the result, write a log, and commit |
| Sunday | 60 minutes | IELTS writing/speaking practice and correction |

Take breaks between blocks. For a busy weekend, reduce to one small exercise and a short log. University coursework takes priority.

## English and the IELTS 7.5 target

Your summer 2025 TOEFL 94 is historical evidence of English experience, not a current IELTS diagnostic or a direct prediction of 7.5. Plan toward February 2027, about five months from this plan's date, while confirming the exact date and required test type/component minimums. Short sample tasks reveal weaknesses but do not establish a reliable overall band. Use a timed full practice test when practical, and obtain calibrated feedback on writing and speaking; AI estimates are only formative.

- Proposed weekdays: 20 minutes on five days, alternating listening with a transcript, reading, vocabulary in sentences, and a short spoken response. Reduce this when university work requires it.
- Saturday English hour: alternate listening and reading tasks, followed by detailed error analysis.
- Sunday English hour: alternate writing and recorded speaking practice. Periodically allocate a longer session to a diagnostic by reducing technical study that week.
- Technical English: a 100–150-word weekly learning log plus a two-minute spoken explanation. Record useful words in sentences; retain Chinese explanations for difficult mathematics when helpful.
- Every four study weekends: reassess one skill using fresh material and adjust the schedule toward the main weakness.

Technical English and IELTS preparation overlap, but exam practice still needs the specific task formats, timing, and scoring criteria. The initial English budget is about three hours 40 minutes per week; the final preparation block raises it to about five hours 40 minutes by reallocating weekend time. These are starting budgets, not guarantees of 7.5. If the diagnostic reveals a larger gap, change the workload or target date rather than assuming this amount is sufficient.

| Calendar period | Main English objective | Evidence and adjustment |
|---|---|---|
| Late September 2026 | Learn IELTS task formats and establish current performance | Timed listening/reading, one writing sample, and a recorded speaking sample; assess each skill separately |
| October 2026 | Repair the two most persistent weaknesses | Maintain an error log; rewrite corrected writing and repeat speaking responses after feedback |
| November 2026 | Build timing and consistency | Weekly timed sections; regular writing and speaking feedback; compare fresh tasks with the baseline |
| December 2026 | Check all four skills and account for university exams | A fuller practice assessment; slow technical work if English needs more time; reduce all optional work during exams |
| January to February 2027 | Exam-specific preparation, especially the final four to six weeks | Allocate four weekend hours to English; timed practice plus detailed review; use several fresh assessments to judge readiness |
| Final week before the booked test | Consolidate and rest | Review recurring errors and test logistics; avoid cramming a new technical project |

For Academic IELTS, alternate Task 1 and Task 2 practice and cover all three Speaking parts over each two-week cycle. Make the allocation more specific after seeing the first samples. Start with the official IELTS sample resource linked above; do not infer a band score from TOEFL alone.

## Daily Python practice and diagnostic

A daily reminder has been scheduled in this Codex task for **12:00 noon**, using the current local timezone (Asia/Shanghai, UTC+8). It proposes a short exercise and asks for the code and explanation. The reminder does not automatically submit solutions to LeetCode or mark exercises as completed. Its difficulty should follow the learner's reported work.

Use [PYTHON-PRACTICE.md](PYTHON-PRACTICE.md) for the initial diagnostic, first seven sessions, and review criteria. Start with loops, lists, strings, dictionaries, sets, functions, and debugging. Add two-pointer methods and simple binary search after these are comfortable. Defer hard dynamic programming and advanced graph problems until there is a concrete need.

The weekly pattern is three new small problems, two reviews or debugging sessions, one mathematical/NumPy bridge exercise, and one short weekly explanation. A daily reminder does not mean seven new problems. Prefer 20 minutes, with an optional extension to 30; on busy days use 10 minutes of review. Weekend sessions count toward the existing implementation time.

Attempt the problem first without a generated solution. Python syntax documentation is allowed. After 15–20 minutes stuck, ask for one hint and record it. Submit the code, time spent, examples tested, and a short explanation. AI feedback should review correctness, reasoning, edge cases, clarity, and time/space complexity. Reattempt the key problem after two days and one week, scheduling reviews inside the existing practice slots rather than adding work.

## Systematic AI-assisted coding

For each experiment: define inputs and expected outputs; attempt the central calculation; request a focused plan or hint; read and run small code changes; check against a hand calculation, known synthetic answer, or baseline; explain and modify the code yourself; record what AI helped with and what you verified.

Example weekly prompt:

> I am on Week [N] of my ML/CV plan. I have [X] hours, and my university deadlines are [...]. I completed [...] but am confused about [...]. I have taken university maths courses, but my ML mathematics is weak: do not assume mastery. Give me one mathematical objective, one small coding output that uses it, and one English output within this budget. Explain mathematics in Chinese if needed and retain key English terms. Define symbols, show the derivation, and use a hand-worked numerical example. Ask diagnostic questions and give hints before full solutions. Finish with three checks I should complete independently.

Example English prompt:

> Correct my learning log while preserving my meaning and level. Explain the three most useful corrections, then ask me to rewrite one sentence myself.

## Recording progress on GitHub

Suggested structure; create folders only when needed:

```text
ML-CV-learning/
  README.md
  STUDY-PLAN.md
  PYTHON-PRACTICE.md
  weekly-log-template.md
  weekly-logs/
  coding-practice/
    README.md
    leetcode/
    math-python/
  notebooks/
  projects/
    image-classification/
    two-view-geometry/
  english/
    vocabulary.md
    writing/
```

Each project should state its question, dataset/source, assumptions, dependencies, run instructions, measured result, and limitations. Attribute adapted code and link to large datasets/course materials. Log understanding and failed experiments as well as successful runs.

Every four study weekends, draft a short supervisor update with what you learned, one demonstrated result, one difficulty, and your next step. Adapt the communication frequency to the supervisor's preference.

## First weekend

- [ ] Reserve a realistic time budget around university work.
- [ ] Use a low-pressure diagnostic to locate gaps in arrays, matrix products, derivatives, probability, and least squares; unknown answers determine what to learn rather than count as failures.
- [ ] Learn vectors, dot products, and norms; calculate a tiny example by hand and repeat it in an existing Python environment or browser notebook.
- [ ] Study one ML introduction and explain data, model, loss, and optimization.
- [ ] Start an English diagnostic and record separate strengths/weaknesses by skill.
- [ ] Write and revise a 100–150-word English log; record a two-minute explanation.
- [ ] Save one notebook and one log with a meaningful commit.
