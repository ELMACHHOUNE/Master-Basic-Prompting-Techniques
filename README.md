# Checkpoint: Master Basic Prompting Techniques

## 1. Zero-Shot Prompt – Email Classification

**Email:**

> "Don't forget the team meeting at 2 PM. Please bring your project updates."

**Classification:**

```text
Work
```

---

## 2. Few-Shot Prompt – Email Classification

**Examples:**

```text
Email: "Dinner at 8 tonight? I’ll bring the wine."
Category: Personal

Email: "You have won a free iPhone! Click here to claim your prize."
Category: Spam

Email: "The Q2 financial report is due by end of day tomorrow."
Category: Work
```

**Email to classify:**

```text
Email: "Are you free for lunch this weekend?"
```

**Solution:**

```text
Personal
```

---

## Conclusion

### Why It Works

**Zero-Shot:**

The model receives instructions without examples. It uses its general understanding of the categories to classify the email.

**Few-Shot:**

The model receives examples showing how emails should be classified. It can use these examples to understand the classification pattern and expected output format.

### Observations

* Zero-shot prompting is simple and flexible.
* Zero-shot prompting may struggle with ambiguous or unusual cases.
* Few-shot prompting provides additional context through examples.
* Few-shot prompting can improve consistency for specific classification tasks.
* Examples should be short, relevant, and diverse.

## Final Answers

| Technique | Email                                                                       | Answer       |
| --------- | --------------------------------------------------------------------------- | ------------ |
| Zero-Shot | "Don't forget the team meeting at 2 PM. Please bring your project updates." | **Work**     |
| Few-Shot  | "Are you free for lunch this weekend?"                                      | **Personal** |
