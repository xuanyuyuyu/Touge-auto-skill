# Problem-type guidance

Read only the section matching the current problem. These are diagnostic priorities, not substitutes for the assignment's exact requirements.

## Algorithm and console programs

- Preserve the required language, file, entry point, and function signature.
- Parse exactly the documented input; print only required output with exact separators, newlines, casing, and numeric precision.
- Check empty/minimum/maximum inputs, duplicates, ordering, overflow, indexing, and time/memory complexity before the final attempt.
- Prefer deterministic sample and boundary tests. Do not add prompts or explanatory text to stdout unless explicitly required.

## HTML, CSS, and JavaScript

- Reproduce visible strings exactly and inspect target images at sufficient zoom.
- Preserve editable markers and write structurally conventional markup; fragile graders may check element order, nesting, attributes, and separate rows or cells rather than appearance alone.
- Follow any explicitly required attribute or declaration order. Do not replace the requested construct with a visually equivalent alternative.
- Before official evaluation, compare the implementation against a compact DOM checklist: required element count and order; exact text and option order; tag nesting; `label[for]` to matching control `id`; shared radio/checkbox `name`; required `value`, `selected`, `checked`, `disabled`, `maxlength`, classes, and inline/style declarations. Distinguish an attribute that must be absent from one that may be empty.
- For forms, prefer explicit label-control association (`label[for]` plus matching `id`) when requested; wrapping a control in a label is not grader-equivalent unless the task permits it.
- If expected output names elements individually but the grader crashes or reports fewer rows, first look for a missing element, wrong tag, wrong order, or an unexpected `value` attribute.
- Treat preview success as non-terminal; require the official grader result.

## SQL and database tasks

- Confirm the database dialect, referenced schema, requested columns, aliases, filtering, grouping, ordering, and duplicate behavior.
- Return only the requested result shape. Check `NULL`, joins, aggregation grain, ties, and deterministic ordering.
- Avoid mutating data unless the problem explicitly requires it and the supplied assignment authorizes that mutation.

## File, shell, and project tasks

- Inspect the provided repository and task instructions before editing. Preserve unrelated user changes.
- Modify only required files and use the requested build/test command when available.
- Distinguish a transient environment failure from a code failure; an evaluation without a valid result does not consume one of the three attempts.

## Interactive or visual tasks

- Inspect the current state and required final state before acting.
- Verify exact labels, control state, ordering, and visible output after each meaningful action.
- Do not trigger purchases, publishing, external messages, destructive actions, or unrelated submissions unless separately authorized.
