# AGENTS.md

This repository is an Obsidian vault for notes related to a Master of Information Systems course.

## Purpose

- Maintain clear, well-structured course notes.
- Prefer edits that improve organization, readability, and long-term retrieval.
- Treat the vault as academic reference material, not application source code.

## Content Guidelines

- Use Markdown files that render cleanly in Obsidian.
- Prefer descriptive note titles and headings.
- Preserve wiki-link style links such as `[[Note Name]]` when useful.
- Keep notes concise, scannable, and well sectioned.
- For lecture notes, prioritise theory, concepts, frameworks, and how the textbook relates to the lecture material.
- Do not capture class case studies, assignment logistics, assessment timelines, group management details, or administrative slide content in lecture notes unless the user explicitly asks.
- Use APA 7 referencing style when references or citations are included.
- When a user provides a source URL for an APA 7 reference, use that URL in the reference instead of replacing it with a DOI link.
- When adding summaries, favor accurate paraphrasing over filler.
- Do not invent citations, quotes, or course facts.
- When the user asks about a specific textbook, chapter, or section, look for the relevant source in the vault assets before answering. Base the answer on that source when available. If the source or requested section cannot be found locally, say so clearly and ask the user to provide the textbook excerpt, screenshot, or file.

## Organization

- Group notes by subject, unit, topic, or assessment when that structure is clear.
- Avoid unnecessary file renames unless they materially improve organization.
- When working on a new asset, rename the file so the relevant week and purpose are easy for both users and agents to find.
- Keep frontmatter optional; only add it when it supports a clear workflow.
- Leave `.obsidian/` configuration alone unless the task is explicitly about vault settings.

## Asset Naming

- Prefer the PISC asset pattern: `Week NN - Descriptive Topic Asset Type.ext`.
- Examples from Professional IS Consulting: `Week 07 - Professional Advice Report Writing Slides.pdf`, `Week 07 - Reesan Report Writing and Workshops Transcript.txt`, `Week 10 - AT2 Risk and Governance Brief.pdf`.
- Put the week first, then the topic, then the asset type such as `Slides`, `Transcript`, `Case Study`, or `Brief`.

## Quiz Notes

- Store quiz notes in the subject-level `Quizzes/` folder, not inside individual `Week NN/` folders.
- Name quiz files by course/week rather than Linear issue key. Prefer `Week NN Quiz.md` within the relevant subject's `Quizzes/` folder, or `PISC - Week NN Quiz.md` / `DBA - Week NN Quiz.md` if subject context is otherwise unclear.
- When a quiz is linked to a Linear issue, record the issue key inside the note, for example `Linear issue: BAJ-104`; do not use the issue key as the default filename unless the user explicitly asks.
- Use the DBA quiz structure as the canonical format:
  - title with week and quiz name;
  - course, source lecture link, Linear issue, and date;
  - `## Scope`;
  - `## Quiz 1`;
  - `### Note-Based Questions`;
  - `### Extension Questions`;
  - `## Answer Template`;
  - `## Grading Notes`;
  - `## User Attempt 1`;
  - note-based score, marking table, extension review, weak areas, revisions made, and extension sources when applicable.
- Questions 1-10 are the note-based quiz and should be based only on the relevant lecture note unless the user gives a broader source scope.
- Questions 11-15 are extension questions. They should be clearly separated from the note-based score and may use external research with APA 7 source notes.
- Do not include an answer key or self-attempt when first creating a quiz for the user unless the user explicitly asks for answers or a demonstration attempt.
- Do not add `## User Attempt`, scores, marking tables, weak areas, or revision outcomes until after the user has actually submitted answers.
- When grading quizzes, be reasonably strict: do not give credit for lazy, vague, or incomplete answers by stretching them to match the expected answer.
- Quiz grading should be less harsh than exam grading, but still require the user's answer to show the key concept, distinction, or reasoning clearly.
- For exams, grade more harshly than quizzes and cite the relevant vault notes more carefully when explaining marks or corrections.
- After the user answers, grade their attempt in the same quiz note, identify weak areas, revise the relevant notes if needed, and create a focused repeat quiz only if the note-based score is below 80%.
- Repeat quiz numbering should continue from the previous quiz's final question number. For example, if the first quiz ended at Q15, the next quiz should start at Q16.
- Repeat quizzes should cover only the topics the user failed or showed weakness on. Do not retest topics they already answered correctly unless needed to check a closely related misconception.

## Linear Planning

- When creating Linear parent issues for assignments, include or ask for the assignment specification, rubric, and case study if one exists.
- Before finalising an assignment parent issue, inspect the vault for the most relevant lecture notes, readings, textbook notes, and assignment assets, then add those references to the issue description.
- If a required specification, rubric, case study, or relevant source cannot be found locally, state the gap clearly and ask the user to provide it.
- Keep assignment parent issues focused on the overall deliverable, source materials, due date, and major workstreams. Put individual assigned sections, review milestones, and submission tasks into child issues.
- When assigning due dates to Linear issues for assignment work, check whether the relevant weekly topic has already been covered in the course notes. Do not schedule a task that depends on a future lecture, reading, or transcript before that topic has been covered unless the user explicitly wants early preparation.
- If an assignment task depends on a topic that has not yet been covered, schedule the task after the relevant weekly note is due, or create a prerequisite note/source-gathering issue first.
- When creating Linear issues for weekly notes, create a quiz child issue for the same due date as the note issue. The quiz is done after the notes are completed.
- Weekly note quizzes should contain 10 questions using a mix of multiple choice and short answer questions, based only on the newly added notes.
- Do not prefix quiz questions with labels such as "Multiple choice:" or "Short answer:". The format should be obvious from whether answer options are present.
- At the end of each weekly note quiz, add 5 additional extension questions that go beyond the notes. Use research to identify relevant concepts, applications, or edge cases not covered in the notes. Keep these separate from the 10 note-based questions and label them clearly as extension questions.
- Do not include extension questions in the 80% note-check score unless the user explicitly asks. The repeat-until-80% workflow applies to the 10 note-based questions only.
- When extension questions rely on external research, cite the sources used in APA 7 style or include a concise source note with stable links where appropriate.
- The quiz workflow is: generate the quiz for the user to answer, wait for the user's responses, grade the user's attempt, identify weak areas, revise the relevant notes if needed, then repeat with another quiz until the user reaches at least 80%.
- Do not answer or self-attempt the user's quiz unless the user explicitly asks for an answer key or demonstration attempt.

### Assignment Parent Issue Template

Use this structure for Linear parent issues for assignments:

```markdown
## Assignment

- Subject:
- Assignment:
- Due:
- Weight:
- Format:

## Required Sources

- Specification:
- Rubric:
- Case study:
- Other brief/assets:

## Relevant Vault Notes

- [[Relevant lecture note]]
- [[Relevant reading note]]
- [[Relevant textbook note]]

## Workstreams

- [ ] Understand the specification and rubric.
- [ ] Read and extract case study requirements, if applicable.
- [ ] Map assignment sections to relevant notes and readings.
- [ ] Draft assigned sections.
- [ ] Review against rubric.
- [ ] Prepare final submission.

## Child Issues To Create

- Assigned sections.
- Research/source gathering.
- Review milestones.
- Final submission task.
```

## Editing Expectations

- Preserve the author's existing writing style where practical.
- Make minimal, targeted changes unless a broader restructure is requested.
- When creating new notes, include enough context that they can stand alone later.
- Prefer plain Markdown over embedded HTML.

## Response Style

- When content has been added directly to Markdown files, do not repeat the full topic details in chat.
- Use chat to briefly state what changed and where, unless the information is not also being written to the vault.

## Course Shorthand

- `DBA` = Digital Business Analysis
- `PISC` = Professional IS Consulting
- `A1` = Assignment 1
- Extend the same pattern for similar assessment shorthand when the meaning is clear from context.

## Git Notes

- The vault is connected to GitHub and may be versioned over time.
- Avoid destructive changes and do not remove note content unless asked.
