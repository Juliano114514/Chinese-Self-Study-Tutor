# Chinese Self-Study Tutor

An adaptive Codex Skill for English- or German-speaking beginners learning Standard Mandarin. It can correct homework, produce model texts, explain grammar and vocabulary, build Hanzi lessons, run quizzes, summarize recurring problems, and lead voice practice.

## Install and invoke

This source package is mirrored to `C:\Users\liangjiayin\.codex\skills\chinese-self-study-tutor`. Codex may select it automatically for Mandarin-learning requests, or you can invoke it explicitly with `$chinese-self-study-tutor`.

Examples:

- `$chinese-self-study-tutor Correct this diary entry at normal depth.`
- `$chinese-self-study-tutor Erkläre mir 把 auf Deutsch, detailed.`
- `$chinese-self-study-tutor full: build a lesson and quiz from 天、地、人.`
- `$chinese-self-study-tutor Practise ordering food with me by voice.`

## Response depth

Choose `quickest`, `simple`, `normal`, `detailed`, or `full`, or let the tutor decide. These are flexible depth preferences rather than strict templates. `normal` and above are automatically archived; input files and requested file outputs default to at least `normal`.

## Archives

Substantial work is saved as self-contained HTML under the active workspace's `archive` directory, grouped into `homework`, `tests`, `knowledge`, `speaking`, and `reviews`. Source files are never modified. Filenames follow `YYYYMMDD Title.html` and `YYYYMMDD [status] Title.html`; collisions receive a numeric suffix rather than being overwritten.

English is the default explanation language. German is used when requested or clearly preferred. The tutor uses Simplified Chinese and tone-marked pinyin by default and can adapt when asked.
