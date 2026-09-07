# Chinese Self-Study Tutor

An adaptive Codex Skill for English-speaking beginners learning Standard Mandarin. It corrects writing, explains grammar and vocabulary, teaches Hanzi through useful words, creates quizzes, reviews recurring problems, and supports voice practice.

Languages: **English** · [Simplified Chinese](docs/i18n/README.zh-CN.md) · [German](docs/i18n/README.de.md)

## Quick start

Installation scope: `user`

Codex can select the Skill automatically for Mandarin-learning requests. To invoke it explicitly:

```text
$chinese-self-study-tutor normal: Correct this diary entry and explain the key mistakes.
```

See the [English quick-start guide](quickstart.txt) for more ready-to-use prompts.

## Choose the response depth

- `quickest`: a direct answer or correction with tone-marked pinyin.
- `simple`: the answer plus the key reason, contrast, or example.
- `normal`: a compact lesson with a Chinese-order breakdown, meaning, focused notes, and short practice.
- `detailed`: deeper comparisons, usage guidance, and targeted practice.
- `full`: a reusable study unit with diagnosis, model material, broader practice, and next steps.

Tone-marked pinyin accompanies the Chinese being taught at every depth unless you ask to omit it. The tutor estimates proficiency conservatively and teaches to the lower plausible level until repeated evidence or an explicit request supports moving higher.

## How corrections are taught

At `normal` and above, composition and correction work can include corrected Chinese, aligned pinyin, a Chinese-order chunk breakdown, a literal gloss, a natural translation, focused notes, and short practice. For example:

```text
我 / 这两天 / 都 / 居家办公
Wǒ / zhè liǎng tiān / dōu / jūjiā bàngōng
I / these two days / all / work from home
Natural English: I have been working from home these past two days.
```

## Hanzi and vocabulary

For an unfamiliar Hanzi, the tutor normally starts with a small network of useful words instead of an isolated dictionary definition. For example, **烛** (*zhú*) can be introduced through **蜡烛** (*làzhú*, wax candle), **烛火** (*zhúhuǒ*, candle flame), **烛光** (*zhúguāng*, candlelight), and **烛台** (*zhútái*, candlestick). This is a flexible teaching approach, not a fixed word-count requirement.

## Defaults and archives

- Explanations are in English by default. You can request German at any time.
- The tutor uses Standard Mandarin, Simplified Chinese, and tone-marked pinyin by default.
- Work at `normal` and above is saved as one self-contained HTML file under the active workspace's `archive` directory.
- Corrections keep the source file unchanged and include the original input, correction, and teaching notes in the same archive file.
- Archive filenames follow `YYYYMMDD [status] Title.html`; a numeric suffix prevents overwriting.

An input file or an explicit request for file output defaults to at least `normal` unless you choose `quickest` or `simple`.
