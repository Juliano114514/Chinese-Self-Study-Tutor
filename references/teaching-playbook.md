# Teaching Playbook

Use this reference to choose useful teaching components. The learner's request always outranks the suggested combinations below.

## Depth selection

Choose depth from the amount of material, the learner's goal, and whether the result should remain useful later.

- **quickest** - Resolve one small question or repair one phrase. Give only the answer needed now, but include tone-marked pinyin for the Chinese taught.
- **simple** - Give the answer with tone-marked pinyin and add the most important reason, contrast, or example. Avoid turning a small question into a lesson handout.
- **normal** - Give a detailed, approachable teaching response. For composition or correction, cover every meaningful sentence with corrected Chinese, tone-marked pinyin, a Chinese-order chunk breakdown, a literal gloss, a natural translation, focused notes, and a short chance to practise. This is the normal floor for input files and requested file outputs.
- **detailed** - Explain form, meaning, Chinese word order, natural alternatives, and recurring patterns. Include targeted practice.
- **full** - Build a self-study unit: diagnosis, teaching, model material, practice, answer handling, review priorities, and a realistic next step.

All depths use tone-marked pinyin for the Chinese being taught unless the learner explicitly asks for no pinyin or another transcription system. Keep the lesson appropriate for the lower of the plausible learner levels unless the learner explicitly requests greater difficulty or has repeatedly demonstrated it. Beyond the required `normal` components, do not mechanically add material that does not help the request.

## Pinyin and structural breakdown

Keep pinyin aligned with the exact Chinese version being taught. Use dictionary tones rather than respelling ordinary tone sandhi unless pronunciation itself is the lesson.

At `normal` or above, show a Chinese-order breakdown for every meaningful corrected sentence or short sentence group. Keep the chunks semantically useful and follow them with a deliberately literal gloss and then a natural translation. For example:

```text
我 / 这两天 / 都 / 居家办公
Wǒ / zhè liǎng tiān / dōu / jūjiā bàngōng
I / these two days / all / work from home
Natural English: I have been working from home these past two days.
```

Do not force English grammar into the literal line: its purpose is to reveal Chinese word order. For long homework, do not skip sentences from the breakdown merely to shorten the response. Closely repeated sentences may share one explanation, but each correction and its pinyin must remain visible.

## Composition and homework correction

Preserve the original text and its section boundaries. Do not silently rewrite facts or personal details.

Possible components, from lighter to deeper:

1. **Corrected wording** - Make the smallest change that repairs grammar, vocabulary, characters, or clarity.
2. **Natural version** - When useful, give a more idiomatic or polished version separately. Label it as an alternative, not the only correct answer.
3. **Pinyin** - Required for the Chinese being taught at every depth unless the learner explicitly opts out.
4. **Structural gloss** - Required at `normal` or above. Break every meaningful corrected sentence into useful chunks and follow Chinese order, even if the learner-language gloss sounds unnatural.
5. **Natural translation** - Translate the intended meaning into clear English or German.
6. **Teaching notes** - Separate definite errors, clarity problems, naturalness, everyday frequency, rhythm, and register. Explain why a form fits this particular context.
7. **Transfer note** - Identify possible English/German transfer only when there is a plausible word-for-word or syntax pattern. Do not label typos or all short sentences as foreign influence.
8. **Model text** - At deeper levels or when requested, provide a new example that uses the same target structures without erasing the learner's voice.
9. **Practice** - Test the actual mistakes or target patterns, not unrelated grammar.

At `normal`, include the original, corrected text, aligned tone-marked pinyin, Chinese-order chunk breakdown with literal gloss, natural translation, focused notes, and a short practice item. At `detailed`, add a minimal-versus-natural comparison, deeper usage contrasts, and more targeted testing. At `full`, add a model text, broader exercise set, problem summary, and follow-up plan.

## Knowledge-point explanations

Start from a concrete Chinese example with tone-marked pinyin, then explain the pattern in the learner's preferred language. At `normal` or above, include a Chinese-order breakdown, literal cue, and natural translation.

Contrast easily confused forms through meaning and situation, not definitions alone. Show what is common in conversation, what is neutral in writing, and what may sound formal, regional, old-fashioned, or unusual. End `normal` or deeper explanations with a small check for understanding.

## Hanzi and vocabulary building

When a learner asks about a single Hanzi, use words and phrases as the main route into the character whenever that is more useful than a standalone dictionary gloss. This is a soft teaching preference: adapt it to the question, and give a direct definition first when the learner specifically needs one.

Start with a familiar anchor word, expand to several common and useful collocations, then briefly draw out the shared character-level idea. If helpful, add a clearly labelled second direction such as a cultural, literary, contrasting, or more specialised word. Keep everyday vocabulary separate from rare or name-like items so a learner does not mistake the latter for basic daily language.

For example, introduce **烛** (*zhú*) through a word network rather than only “candle”:

- **蜡烛** (*làzhú*) — wax candle; a familiar anchor word.
- **烛火** (*zhúhuǒ*) — candle flame.
- **烛光** (*zhúguāng*) — candlelight.
- **烛台** (*zhútái*) — candlestick / candle holder.
- **烛龙** (*Zhúlóng*) — Torch Dragon; a literary or mythological name, not everyday vocabulary.

The first four words show the everyday candle-and-light network. The last word offers a second cultural direction and should be labelled as such. Only after the network is visible, state the compact character-level cue: **烛** (*zhú*) commonly carries the image of a candle or torch in these words.

Use several terms when they make the network clearer, not to meet a fixed count. Do not pad with rare words, and do not infer one universal English equivalent from a character that has different senses in different compounds. Read [hanzi-teaching.md](hanzi-teaching.md) for the fuller reference and worked patterns.

A useful entry may contain:

- word or phrase in Hanzi;
- tone-marked pinyin;
- character-by-character or morpheme cue, clearly marked as a memory aid rather than a complete etymology;
- exact everyday meaning and relevant register;
- one short beginner-readable example with translation.

Group semantic families, contrasting uses, or reusable patterns when this makes recall easier. At `normal` or deeper, add recognition, matching, multiple-choice, cloze, or short-production practice and explain the answers after the learner attempts them.

## Quizzes and answer handling

Build quizzes from material already taught or supplied. Mix recognition and production according to the learner's level. Keep distractors plausible but unambiguous.

- In conversation, present questions without the answer key. After the learner answers, mark each response, explain the decisive point, and offer a retry where useful.
- For a one-shot self-study package, create a separate `[quiz]` artifact and `[answer-key]` artifact so answers are easy to hide.
- A score is optional. Prefer a short diagnosis such as "secure", "needs one more pass", or "confused with X" over false precision.
- Add tone-marked pinyin to Chinese prompts, options, corrections, and answer explanations unless the learner explicitly opts out.

## Voice and speaking practice

Choose a practical scenario such as introductions, ordering food, directions, travel, daily routines, or talking with a friend. Establish the goal briefly, then conduct one Mandarin turn at a time. Use English or German scaffolding only as needed.

Do not interrupt every sentence. During the exchange, prioritize communication and repair only errors that block meaning or reinforce the current target. Afterward, summarize a small number of high-value corrections, useful replacement phrases, vocabulary, and the next speaking target.

Add tone-marked pinyin to Chinese text shown during speaking practice and in the review unless the learner explicitly opts out.

Only evaluate sounds, tones, fluency, or rhythm that were actually available in the audio. If audio evidence is missing or unclear, say so and assess wording instead. At archive-eligible depth, save a concise speaking review, not raw audio or a full transcript, unless the user explicitly requests those materials.

## Progress reviews

At `full` depth or on request, look across a small set of recent relevant archives. Group recurring issues by useful learning target, cite representative learner sentences, show corrected patterns, acknowledge improvement, and recommend the next few priorities. Do not infer a broad proficiency level from one task.
