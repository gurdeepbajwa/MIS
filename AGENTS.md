# AGENTS.md

This repository is a Zed-based Markdown workspace for notes related to a Master of Information Systems course.

## Purpose

- Maintain clear, well-structured course notes.
- Prefer edits that improve organization, readability, and long-term retrieval.
- Treat the workspace as academic reference material, not application source code.

## Content Guidelines

- Use Markdown files that render cleanly in Zed's Markdown preview.
- Prefer descriptive note titles and headings.
- Preserve wiki-link style links such as `[[Note Name]]` when useful.
- Keep notes concise, scannable, and well sectioned.
- For lecture notes, prioritise theory, concepts, frameworks, and how the textbook relates to the lecture material.
- Do not capture class case studies, assignment logistics, assessment timelines, group management details, or administrative slide content in lecture notes unless the user explicitly asks.
- Use APA 7 referencing style when references or citations are included.
- When a user provides a source URL for an APA 7 reference, use that URL in the reference instead of replacing it with a DOI link.
- When adding summaries, favor accurate paraphrasing over filler.
- Do not invent citations, quotes, or course facts.
- When the user asks about a specific textbook, chapter, or section, look for the relevant source in the workspace assets before answering. Base the answer on that source when available. If the source or requested section cannot be found locally, say so clearly and ask the user to provide the textbook excerpt, screenshot, or file.
- For assignment reports, use an academic technical-report tone while keeping the language natural and readable. Prefer precise business-analysis language over marketing copy or casual phrasing. Avoid informal implementation labels such as "big-bang rollout"; use terms such as "single-stage deployment", "phased implementation", "incremental delivery", or "iterative refinement" where appropriate.

## Organization

- Group notes by subject, unit, topic, or assessment when that structure is clear.
- Avoid unnecessary file renames unless they materially improve organization.
- When working on a new asset, rename the file so the relevant week and purpose are easy for both users and agents to find.
- Keep frontmatter optional; only add it when it supports a clear workflow.
- Leave `.zed/` editor configuration alone unless the task is explicitly about editor settings.

## Asset Naming

- Prefer the PISC asset pattern: `Week NN - Descriptive Topic Asset Type.ext`.
- Examples from Professional IS Consulting: `Week 07 - Professional Advice Report Writing Slides.pdf`, `Week 07 - Reesan Report Writing and Workshops Transcript.txt`, `Week 10 - AT2 Risk and Governance Brief.pdf`.
- Put the week first, then the topic, then the asset type such as `Slides`, `Transcript`, `Case Study`, or `Brief`.

## Lecture Note Structure

- Split lecture notes into course-sourced material and supplemental material.
- Course-sourced sections should be based on the lecture, transcript, and assigned readings.
- When writing or revising notes, check whether each section is fleshed out clearly enough from the course sources.
- If a section needs more explanation, add an `Extra Materials` subheading inside that section and place supplemental explanation, examples, or outside resources there.
- Keep supplemental material clearly separated from lecture, transcript, and reading content so it is obvious what came from the course and what was added for study support.

## Diataxis Organization

- Use Diataxis lightly as an organizing model when it helps make notes easier to retrieve.
- Treat lecture notes, definitions, models, frameworks, and key facts as reference material.
- Treat conceptual background, reasoning, comparisons, and "why this matters" content as explanation material.
- Treat assignment workflows, report-writing processes, analysis methods, and repeatable study tasks as how-to material.
- Treat practice quizzes, worked examples, and guided exercises as tutorial material.
- Do not force every note into a Diataxis category, but use the distinction to avoid mixing reference, explanation, how-to guidance, and practice material when separation would make the workspace clearer.
- When a lecture contains an applied framework, method, model, or theory that may be used in exams or assignments, create a separate same-week Diataxis note when useful rather than overloading the lecture note.
- Place same-week Diataxis notes in the relevant `Week NN/` folder and link them from the parent `Lecture.md` under `## Applied Diataxis Notes`.
- Choose `How-to guide` for applying a method to a scenario, `Reference` for concise lookup tables or definitions, `Tutorial` for a guided worked example, and `Explanation` for deeper theory, limitations, assumptions, or conceptual connections.
- Diataxis notes should not duplicate the full lecture note. They should focus on application, lookup, practice, or explanation and link back to the source lecture.

## Extra Resources

- When finding YouTube videos for a lecture, extract the lecture's key points first and use those concepts as the search basis.
- Prefer high-quality, relevant videos that explain the lecture's main theories, frameworks, methods, or practical applications.
- Do not recommend loosely related videos just because they share a keyword with the lecture.
- Add selected videos under the relevant section's `Extra Materials` subheading, or in a clearly named extra-resources note if the material spans multiple sections.
- Include enough source detail for later retrieval: title, channel, URL, and the lecture topic or week it supports.

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
- For new weekly quizzes, use a retrieval-first exam-prep structure where practical:
  - questions 1-3 test core recall and recognition from the new lecture note;
  - questions 4-6 test distinctions between similar concepts;
  - questions 7-8 apply the week's concepts to short scenarios;
  - question 9 asks the user to critique or correct a weak answer, recommendation, or analysis;
  - question 10 asks for a short written exam-style answer.
- Add a separate `### Delayed Review Questions` section after the extension questions when useful. These questions should revisit earlier weeks for spacing and interleaving, and should not count toward the 80% note-check score unless the user explicitly asks.
- Do not include an answer key or self-attempt when first creating a quiz for the user unless the user explicitly asks for answers or a demonstration attempt.
- Do not add `## User Attempt`, scores, marking tables, weak areas, or revision outcomes until after the user has actually submitted answers.
- When grading quizzes, be reasonably strict: do not give credit for lazy, vague, or incomplete answers by stretching them to match the expected answer.
- Quiz grading should be less harsh than exam grading, but still require the user's answer to show the key concept, distinction, or reasoning clearly.
- When grading each quiz answer, create and apply a short per-question rubric before assigning the mark. The rubric should state what earns full credit, partial credit, and no credit for that specific question.
- Score each note-based answer from `0.0` to `1.0`, including partial and brief answers. Use decimals where needed rather than rounding vague answers up to full marks.
- Use this default quiz scoring scale unless the question requires a more specific rubric:
  - `1.0`: Correct and complete; clearly shows the key concept, distinction, or reasoning required.
  - `0.75`: Mostly correct; minor omission, imprecision, or wording issue, but the core idea is clear.
  - `0.5`: Partly correct; shows some relevant understanding but misses an important part of the concept or distinction.
  - `0.25`: Minimal credit; contains a relevant fragment or keyword but does not explain the concept adequately.
  - `0.0`: Incorrect, blank, contradicted by the notes, or too vague to show understanding.
- In the marking table, include a `Rubric` column or include the rubric inside the feedback cell for each question. The user should be able to see why a partial answer received its exact score.
- For exams, grade more harshly than quizzes and cite the relevant workspace notes more carefully when explaining marks or corrections.
- After the user answers, grade their attempt in the same quiz note, identify weak areas, revise the relevant notes if needed, and create a focused repeat quiz only if the note-based score is below 80%.
- Repeat quiz numbering should continue from the previous quiz's final question number. For example, if the first quiz ended at Q15, the next quiz should start at Q16.
- Repeat quizzes should cover only the topics the user failed or showed weakness on. Do not retest topics they already answered correctly unless needed to check a closely related misconception.
- Create milestone exams after major topic blocks have been covered. Milestone exams should be placed in the subject-level `Quizzes/` folder, named `Milestone Exam NN - Descriptive Topic.md`, and scheduled after a delay of roughly two to three weeks where possible so they test retention rather than immediate familiarity.
- Create full-semester practice exams in the subject-level `Quizzes/` folder, named `Practice Exam NN - Full Semester.md`. These should be closed-book, written, scenario-heavy, and should not include answer keys unless the user explicitly asks.

## Linear Planning

- When creating Linear parent issues for assignments, include or ask for the assignment specification, rubric, and case study if one exists.
- Before finalising an assignment parent issue, inspect the workspace for the most relevant lecture notes, readings, textbook notes, and assignment assets, then add those references to the issue description.
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

## Relevant Workspace Notes

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
- Use chat to briefly state what changed and where, unless the information is not also being written to the workspace.

## Course Shorthand

- `DBA` = Digital Business Analysis
- `PISC` = Professional IS Consulting
- `A1` = Assignment 1
- Extend the same pattern for similar assessment shorthand when the meaning is clear from context.

## Git Notes

- The workspace is connected to GitHub and may be versioned over time.
- Avoid destructive changes and do not remove note content unless asked.
