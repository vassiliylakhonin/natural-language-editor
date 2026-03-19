# Natural Language Editor

Rewrite text so it sounds natural, clear, and human — without changing meaning or facts.

## What this skill does

`natural-language-editor` helps polish drafts by removing robotic phrasing, improving flow, and tightening wording while preserving intent.

### Best for
- Polishing rough drafts
- Removing AI-like phrasing
- Improving readability
- Shortening text without losing meaning
- Making writing more professional

## Install

From ClawHub:

```bash
clawhub install natural-language-editor
# or pin version
clawhub install natural-language-editor --version 1.0.1
```

## Usage

### Modes
- `edit [text]` — natural rewrite (default)
- `edit --concise [text]` — shorter, same meaning
- `edit --clarity [text]` — easier to understand
- `edit --professional [text]` — polished, neutral tone
- `edit --light [text]` — minimal edits
- `edit --deep [text]` — stronger restructuring, same meaning
- `edit --anti-ai [text]` — reduce templated/robotic cadence
- `edit --json [text]` — structured output

## Example

Input:

> This solution plays a crucial role in modern society and significantly contributes to improved outcomes.

Output:

> This solution is widely used today and helps improve results.

## Guarantees

- Preserves meaning
- Does not add new facts
- Keeps essential claims
- Avoids injecting new opinions or emotions
- Keeps technical terms when precision matters

## JSON Output (`--json`)

```json
{
  "issues_found": ["repetitive phrasing", "inflated language"],
  "rewrite_strategy": "remove filler and simplify wording",
  "rewritten_text": "...",
  "introduced_subjectivity": false
}
```

## Changelog

### 1.0.1
- Added `--anti-ai` mode
- Tightened rewrite validation workflow

### 1.0.0
- Initial clean release
- Normalized frontmatter and structure
