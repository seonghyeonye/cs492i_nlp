# korquad-open-cs492I
KorQuad-Open Baseline Code for KAIST CS492I 2020 Fall

## Original Author
Seonhoon Kim (Naver)

## Train in NSML
```bash
sh run_nsml.sh
```

## Train in Local

```bash
sh run_local.sh
```

## How to Improve?

### How to select the best answer among different contexts.

We deal with a QA task with a single question and multiple contexts (i.e., paragraphs). One of the most important issues in this type of task is in which paragraph to pick the answer span. Current naive implementation is comparing the probability in a prediction and choosing the paragraph with the largest. Implement a strategy to pick the best answer.

**NOTE: In the baseline, the f1-score for the validation is measured per paragraph, and the f1-score for the test is measured per question.**

### How to select training samples considering a memory limit.

There are multiple contexts, but since there is a memory limit, we cannot include everything in training. The baseline is using first three samples in sequence. Which training samples should we choose to learn the best representation? 

### Change model and hyper-parameter configurations.

Do as much as you want.