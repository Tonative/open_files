# NaijaHealth Benchmark (Preview Sample)

A healthcare benchmarking dataset for evaluating LLM performance on medical queries across three Nigerian languages — **Pidgin**, **Hausa**, and **Igbo**.

Each entry pairs an English health prompt (single-turn or multi-turn clinical conversations) with human translations, alongside a scored rubric tailored to the Nigerian healthcare context and covering local disease prevalence, available resources, and clinical practice norms.

## Data structure

Each JSON entry contains:

- **`prompt_id`** — unique identifier for the prompt scenario
- **`prompts`** — English prompt text(s) with turn labels
- **`languages`** — human translations in Pidgin, Hausa, and Igbo
- **`rubric`** — Nigerian-context evaluation criteria with positive/negative scores

```json
{
  "prompt_id": "92fb3dc3-...",
  "prompts": [{"label": "Prompt", "text": "switching to a biologic therapy..."}],
  "languages": {
    "Pidgin": "dey change to one kind treatment wey dey boost immune....",
    "Hausa": "na koma amfani da maganin gargajiya...",
    "Igbo": "na-agbanwe gaa na ọgwụgwọ ọhụrụ..."
  },
  "rubric": [
    {"criteria": "Mentions the risks and side effects...", "score": 10.0},
    {"criteria": "Writes a long and hard-to-follow answer...", "score": -2.0}
  ]
}
```

## Languages

| Language | ISO 639 | Speakers (approx.) |
|----------|---------|---------------------|
| Nigerian Pidgin | pcm | 75M+ |
| Hausa | ha | 80M+ |
| Igbo | ig | 45M+ |

## License

This preview sample is released under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/). You are free to share it for non-commercial purposes, but derivatives and commercial use are not permitted.

## Full dataset

This is a preview of a larger commercial dataset. If you're interested in accessing the full version that contains more Nigerian languages such as Fula and Yoruba, and more data records, please reach out via the contact details below.

## Contact

<!-- Replace with your preferred contact method -->
📧 [services@tonative.org](mailto:services@tonative.org)
