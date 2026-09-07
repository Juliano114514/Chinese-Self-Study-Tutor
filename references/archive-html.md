# Archive and HTML Contract

Read this reference before writing an archive artifact.

## Archive root and categories

Use `archive/` under the active workspace, not inside the installed Skill directory. Create only the category directories needed for the current task.

- `archive/homework/` - meaningful learner input, `[corrected]`, and `[model-answer]`
- `archive/tests/` - `[quiz]` and `[answer-key]`
- `archive/knowledge/` - `[lesson]`
- `archive/speaking/` - `[speaking-review]`
- `archive/reviews/` - `[progress-review]`

Keep related input and correction in `homework`. Put a quiz generated from homework in `tests`; include the source title in its metadata so the relationship stays clear.

## Filenames

Use the active workspace's local calendar date in `YYYYMMDD` form.

- Normalized source: `YYYYMMDD Title.html`
- Result: `YYYYMMDD [status] Title.html`

Supported status words are descriptive defaults, not an exhaustive list: `corrected`, `model-answer`, `quiz`, `answer-key`, `lesson`, `speaking-review`, and `progress-review`.

Choose the title in this order:

1. a title explicitly supplied by the user;
2. the input filename without its extension;
3. a short descriptive title derived from the task, in the current explanation language when practical.

Remove Windows-invalid filename characters (`< > : " / \\ | ? *`), control characters, and trailing spaces or periods. Keep meaningful Unicode, including Hanzi. Do not repeat an existing leading date from the source name; the archive date is today's date.

Never overwrite. If a target exists, append ` (2)`, then ` (3)`, and so on before `.html`. Apply collision handling independently to each artifact.

## What to archive

- At `normal`, `detailed`, or `full`, archive automatically.
- At `quickest` or `simple`, archive only after an explicit save request.
- If the user supplies a file or asks for a file output without naming a depth, use at least `normal`.
- Preserve every source file unchanged. The normalized source HTML is an archival representation, not a replacement or move.
- For pasted homework or another meaningful learner text, create a source HTML and the related result HTML.
- For a pure knowledge request, archive the `[lesson]` result and include the original question in its metadata; a separate source file is unnecessary.
- For speaking, archive a concise `[speaking-review]`; omit audio and full transcript unless explicitly requested.

## Self-contained HTML

Write UTF-8 HTML5 with `lang` set to the main explanation language (`en`, `de`, or `zh-CN`). Use a short embedded `<style>` block, system font stacks that include Chinese-capable fonts, and no scripts, remote stylesheets, web fonts, trackers, or external media.

Use semantic headings and readable vertical sections rather than forcing tables. A typical artifact includes:

- title;
- local date, depth, category, explanation language, and source filename or related artifact when relevant;
- learner input or question;
- the teaching content appropriate to the task;
- practice or next step when useful.

For corrected work, visually distinguish original, minimally corrected, and natural/model alternatives. Do not rely on color alone; label every section in text. Keep line wrapping comfortable, contrast high, and print output clean. Include `@media print` rules and avoid fixed-height containers that can clip text.

Escape source text before inserting it into HTML. Preserve intentional paragraph and section breaks. If text extraction from PDF, image, audio, or another source is incomplete, mark the uncertainty in the archive instead of silently guessing.

Before reporting success, reopen or parse each written file and confirm:

- valid UTF-8 and recognizable HTML structure;
- expected title, date, depth, and content are present;
- no replacement characters caused by encoding loss;
- no `<script>`, remote resource, or accidental answer key in an interactive quiz;
- the exact final path does not replace an earlier artifact.
