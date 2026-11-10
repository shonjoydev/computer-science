# 🤝 Contributing to Computer Science

Thank you for helping improve this computer science knowledge base. Contributions that make the material more accurate, understandable, useful, and maintainable are welcome.

## 1. Ways to Contribute

You can contribute by:

- Correcting technical inaccuracies or broken links.
- Improving explanations, examples, and diagrams.
- Adding exercises, tests, or practical implementations.
- Suggesting books, research papers, courses, and official documentation.
- Improving learning roadmaps and prerequisite relationships.
- Adding projects or documenting experiments.
- Improving accessibility, navigation, and consistency.
- Reporting unclear, incomplete, or outdated material.

## 2. Before Making a Change

1. Read the relevant topic documentation.
2. Check whether the topic already exists elsewhere in the repository.
3. Open an issue for substantial structural changes or large additions.
4. Prefer focused changes that are easy to review.
5. Check the license and usage terms of any external material.

## 3. Documentation Standards

- Write explanations in your own words.
- Define unfamiliar terminology.
- Introduce prerequisites where they matter.
- Use examples to clarify abstract concepts.
- Distinguish facts, assumptions, interpretations, and opinions.
- Cite reliable sources for claims that need evidence.
- Prefer textbooks, peer-reviewed research, official documentation, and primary sources when appropriate.
- Do not copy substantial portions of copyrighted books, courses, or websites.
- Use diagrams when they materially improve understanding.
- Keep links relative when linking to files inside this repository.

## 4. Code Standards

- Prefer readable, maintainable code over clever shortcuts.
- Use Python for DSA examples unless another language is required by the subject.
- Include meaningful names, docstrings, and comments where useful.
- Explain important algorithmic choices.
- Include tests for expected behavior and edge cases.
- State time and space complexity for algorithm implementations.
- Avoid committing secrets, credentials, personal data, generated binaries, or unrelated files.
- Include instructions for running non-trivial examples.

## 5. Folder and File Naming

- Preserve the established numbered top-level directory names.
- Use descriptive kebab-case names for new topic folders.
- Use clear names for documentation files.
- Use numbered prefixes for sequential chapter notes when they improve navigation.
- Do not rename or move established folders without updating all affected links and documentation.

**Naming principle:** Folder names identify what the content is; documentation explains when and how to learn it.

## 6. Suggested Topic Documentation Structure

Use this as a starting point, adapting it to the subject:

```text
topic-name/
├── README.md
├── concepts/
├── examples/
├── exercises/
├── implementations/
├── diagrams/
└── references.md
```

A topic README may include:

1. Overview and learning objectives.
2. Prerequisites.
3. Core concepts and terminology.
4. Worked examples.
5. Algorithms, proofs, or implementation details where relevant.
6. Common mistakes and edge cases.
7. Exercises and projects.
8. Connections to related topics.
9. References and further reading.

Do not create empty folders merely to match this template.

## 7. Pull Request Checklist

Before submitting a pull request, check:

- [ ] The change has a clear purpose.
- [ ] The relevant topic or folder is the correct location.
- [ ] Explanations are original and technically accurate.
- [ ] External sources are cited where appropriate.
- [ ] Code examples run and tests pass, where applicable.
- [ ] Relative links and images work.
- [ ] Markdown tables and code fences render correctly.
- [ ] No secrets, credentials, or unrelated generated files are included.
- [ ] Related navigation and roadmap documents are updated.

## 8. Commit Messages

Use short, descriptive commit messages. Examples:

```text
docs: clarify binary search prerequisites
docs: add graph traversal examples
feat: add heap implementation in Python
test: cover empty-tree traversal cases
fix: correct database normalization link
```

## 9. Issues and Discussions

When reporting a problem, include:

- The file or topic affected.
- What is incorrect, missing, or unclear.
- Why the change would improve the repository.
- A source or example when it helps establish the issue.

For code defects, include a minimal reproducible example when possible.

## 10. Respectful Collaboration

Be constructive and respectful. Focus reviews on the work, explain technical disagreements with evidence, and welcome different valid approaches.

Thank you for helping make this resource more useful for learners.
