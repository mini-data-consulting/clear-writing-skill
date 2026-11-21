# clear-writing

An agent skill that makes your agent write plain, readable prose. It applies five standard references, each to one level of the text.

| Level | Reference | Main rule |
|---|---|---|
| Document | ISO 24495-1:2023 (plain language) | Readers can get, find, understand and use what they need |
| Paragraph | Joseph Williams, *Style: Lessons in Clarity and Grace* | Each sentence opens with what the reader knows and ends with what is new |
| Sentence | Strunk and White, *The Elements of Style* | Each sentence carries one idea, in the active voice |
| Word | Garner's Modern English Usage | Use plain words, and keep one term for each concept |
| Requirement | RFC 2119 and RFC 8174 | MUST, SHOULD and MAY appear in uppercase, and only in text that sets rules |

## When it runs

The agent loads the skill when it writes docs, READMEs, specs, guides, emails, PR descriptions, help text, error messages or instruction files. It also loads when you ask the agent to make writing clearer or tighter.

## How it revises

The skill revises from the document down to the word. That way the agent never polishes a section it later cuts.

## Install

```bash
npx skills add mini-data-consulting/clear-writing-skill
```

You can also copy `skills/clear-writing/` into `.claude/skills/` in a project, or into `~/.claude/skills/` for yourself.

## Your rules win

Any style rules you give your agent override this skill.

## License

0BSD. Use it however you like.
