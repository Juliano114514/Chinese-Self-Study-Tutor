# Chinese Self-Study Tutor

An adaptive Codex Skill for English- or German-speaking beginners learning Standard Mandarin. It can correct homework, produce model texts, explain grammar and vocabulary, build Hanzi lessons, run quizzes, summarize recurring problems, and lead voice practice.

Other languages: [简体中文 README](docs/i18n/README.zh-CN.md) · [中文快速开始](docs/i18n/quickstart.zh-CN.txt) · [Deutsche README](docs/i18n/README.de.md) · [Deutscher Schnellstart](docs/i18n/quickstart.de.txt)

## Install and invoke

This source package is mirrored to `C:\Users\liangjiayin\.codex\skills\chinese-self-study-tutor`. Codex may select it automatically for Mandarin-learning requests, or you can invoke it explicitly with `$chinese-self-study-tutor`.

Examples:

- `$chinese-self-study-tutor Correct this diary entry at normal depth.`
- `$chinese-self-study-tutor Erkläre mir 把 auf Deutsch, detailed.`
- `$chinese-self-study-tutor full: build a lesson and quiz from 天、地、人.`
- `$chinese-self-study-tutor Practise ordering food with me by voice.`

## Response depth

Choose `quickest`, `simple`, `normal`, `detailed`, or `full`, or let the tutor decide. These are flexible depth preferences rather than strict templates. `normal` and above are automatically archived; input files and requested file outputs default to at least `normal`.

Tone-marked pinyin accompanies the Chinese taught at every depth unless you explicitly ask for no pinyin. The tutor estimates proficiency conservatively and teaches to the lower plausible level until repeated evidence or an explicit request supports moving higher.

At `normal`, composition and correction work includes a sentence-by-sentence learning view: corrected Chinese, aligned pinyin, a Chinese-order chunk breakdown and literal gloss, a natural translation, focused notes, and short practice. For example:

```text
我 / 这两天 / 都 / 居家办公
Wǒ / zhè liǎng tiān / dōu / jūjiā bàngōng
I / these two days / all / work from home
Natural English: I have been working from home these past two days.
```

## Hanzi and vocabulary

For an unfamiliar Hanzi, the tutor normally starts with a useful word network rather than an isolated dictionary definition. For example, **烛** (*zhú*) can begin with **蜡烛** (*làzhú*, wax candle), **烛火** (*zhúhuǒ*, candle flame), **烛光** (*zhúguāng*, candlelight), and **烛台** (*zhútái*, candlestick). A second, clearly labelled cultural direction—such as **烛龙** (*Zhúlóng*, Torch Dragon)—can help when relevant. This is a flexible reference, not a fixed word count or a replacement for direct explanation.

## Archives

Substantial work is saved as self-contained HTML under the active workspace's `archive` directory, grouped into `homework`, `tests`, `knowledge`, `speaking`, and `reviews`. Source files are never modified. Filenames follow `YYYYMMDD Title.html` and `YYYYMMDD [status] Title.html`; collisions receive a numeric suffix rather than being overwritten.

English is the default explanation language. German is used when requested or clearly preferred. The tutor uses Simplified Chinese and tone-marked pinyin by default and can adapt when asked.
