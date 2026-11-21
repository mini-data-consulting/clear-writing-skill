---
name: clear-writing
description: Plain-language rules for any prose meant for a reader, built on ISO 24495-1 (plain language), Garner's Modern English Usage (words), Strunk and White (sentences), Joseph Williams' Style (paragraphs) and RFC 2119 (requirement keywords). Use it whenever you write or revise docs, READMEs, specs, guides, emails, PR descriptions, blog posts, help text, error messages, skill files or CLAUDE.md instructions, or when the user asks to make writing clearer, tighter, plainer or easier to follow.
---

# Clear writing

Readers came for something. Give it to them, then stop.

The standards apply in layers. The document as a whole follows ISO 24495-1. Paragraphs follow Williams. Sentences follow Strunk and White. Words follow Garner. Requirement keywords follow RFC 2119.

## 1. The document: ISO 24495-1:2023

The plain-language standard calls a document plain when its readers can:

1. **Get what they need.** Before writing, name the reader and the task they bring. Cut whatever does not serve that task, however true or hard-won it is.
2. **Find what they need.** Put the answer or the main point first. Write headings that say what the section holds ("Rotate an API key", not "Overview"). Keep related facts together. Use lists for steps and parallel items, tables for comparisons.
3. **Understand what they find.** Use words the reader already knows. Define a term the first time it appears, then keep using that same term. Show an example where an abstraction might lose them.
4. **Use the information.** Steps go in the order the reader does them, one action per step. Name the result they should see, so they know a step worked. End with what to do next, or nothing.

Run these four checks on every draft before polishing a single sentence.

## 2. Paragraphs: Williams, *Style: Lessons in Clarity and Grace*

- **Old before new.** Open each sentence with what the reader already knows, from the last sentence or from the context. Close it with what is new. The new idea at the end becomes the known idea that opens the next sentence, and the paragraph flows.
- **Stress at the end.** The last words of a sentence carry the weight. Put the important, new or complex information there, not a trailing qualifier.
- **Characters as subjects, actions as verbs.** Name who acts and make them the subject. Turn nominalizations back into verbs: "the validation of the input is performed by the parser" becomes "the parser validates the input".
- **Consistent topic strings.** Keep the subjects of a paragraph's sentences pointing at the same few characters. When the subject jumps around, the reader loses the thread.
- **Point first.** State the paragraph's point in its first sentence or two. Supporting detail follows.
- **Short subjects, early verbs.** Get to the main verb quickly. A long subject makes the reader hold too much before learning what happened.

## 3. Sentences: Strunk and White, *The Elements of Style*

- **One idea per sentence.** A sentence may be short or long. Its length follows the idea it carries, never the other way around.
- **Omit needless words.** Each word does work or goes. "In order to" becomes "to"; "the fact that he had not arrived" becomes "his failure to arrive"; "at this point in time" becomes "now".
- **Active voice** unless the actor is unknown or irrelevant.
- **Positive form.** Say what is, not what isn't: "forgot", not "did not remember"; "late", not "not on time".
- **Specific and concrete.** Prefer "the build fails on Node 18" to "there may be compatibility concerns".
- **Parallel form** for parallel ideas, especially in lists and headings.
- **Keep related words together.** Place modifiers next to what they modify.
- **Emphatic words at the end.** This rule and Williams' stress position say the same thing.

## 4. Words: Garner's Modern English Usage

- **Plain over pompous.** "Use", not "utilize"; "about", not "with regard to"; "before", not "prior to"; "help", not "facilitate"; "start", not "commence".
- **Precise over approximate.** Know the difference in each confusable pair: affect/effect, comprise/compose, fewer/less, imply/infer, which/that (restrictive clauses take "that" in American English), ensure/insure.
- **Avoid skunked words.** When a word's meaning is in dispute ("decimate", "literally", "hopefully" meaning "I hope"), whichever sense you intend will distract some readers. Pick a different word.
- **Cut redundancies.** "Past history", "future plans", "end result", "completely eliminate", "free gift".
- **Cut hedges and intensifiers.** "Very", "really", "quite", "basically", "simply", "just", "actually" rarely add meaning.
- **One term per concept.** Once you call it a "workspace", do not later call it a "project" or "account" to vary the prose. Readers assume a new word means a new thing.
- **Prefer the reader's words** over internal jargon or code names.

When unsure of a usage, follow Garner's verdict: the form careful writers use today, not the oldest form or the loosest one.

## 5. Requirement keywords: RFC 2119 (with RFC 8174)

Use these only in specs, instructions, policies, skill files, CLAUDE.md files and other text that sets requirements.

| Keyword | Meaning |
|---|---|
| MUST / REQUIRED / SHALL | Absolute requirement |
| MUST NOT / SHALL NOT | Absolute prohibition |
| SHOULD / RECOMMENDED | Do it unless you have a valid reason not to, and understand the cost |
| SHOULD NOT / NOT RECOMMENDED | Avoid it unless you have a valid reason, and understand the cost |
| MAY / OPTIONAL | Truly optional |

- The words carry this meaning only in UPPERCASE (RFC 8174). Lowercase "must" is ordinary English.
- Use them sparingly. A page where everything is a MUST tells the reader nothing about priority.
- Give the reason behind a requirement when the reason is not obvious. A reader who understands the why applies the rule to cases you did not foresee.
- In a formal spec, state the convention near the top: "The key words MUST, MUST NOT, SHOULD, SHOULD NOT and MAY are to be read as described in RFC 2119 and RFC 8174."
- Never use the keywords in marketing or conversational copy.

## How to revise

Revise in this order, coarse to fine. Fixing words in a section that should be cut wastes the effort.

1. **Document.** Run the four ISO checks. Cut, reorder, re-head.
2. **Paragraphs.** Confirm each opens with its point and flows from old information to new.
3. **Sentences.** Find the character and the action in each. Make them subject and verb. Split any sentence that carries two ideas.
4. **Words.** Replace pompous, vague, redundant and skunked words. Check that each term stays the same throughout.
5. **Read it as the reader.** Can they find the answer in ten seconds? Can they act on it without asking you a question?

## Also apply

- The user's own style rules win over this skill.
- Do not announce the structure ("In this section we will..."). Use a heading instead.
- When editing someone else's text, keep their voice and meaning. Change what is unclear, not what is merely different from how you would say it.
