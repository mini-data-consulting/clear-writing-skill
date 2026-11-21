---
name: clear-writing
description: Plain-language writing rules from ISO 24495-1, Joseph Williams' Style, Strunk and White, Garner's Modern English Usage and RFC 2119. Use it when writing or revising prose that someone will read, such as docs, READMEs, specs, guides, emails, PR descriptions, blog posts, help text, error messages and agent instructions. Also use it when asked to make writing clearer or plainer.
---

# Clear writing

Write so that readers can find what they came for and act on it. Name the reader and their task first. Then draft, and revise in four passes, from the whole document down to single words. Each pass follows one reference work.

## Before you draft

Name the reader and the task they bring. A developer setting up a project needs the commands in order. A manager choosing a vendor needs the recommendation and its cost. Everything in the text serves that task. Anything else comes out, however true it is.

## Pass 1: Shape the document (ISO 24495-1)

The plain-language standard ISO 24495-1:2023 calls a document plain when its readers can get what they need, find it, understand it and use it. Check each in turn.

- **Get.** Cut every section the reader's task does not need.
- **Find.** Put the answer first. Write headings that name what a section holds: "Rotate an API key" tells the reader more than "Overview". Let the heading introduce the section, so the text never announces itself ("In this section we will..."). Use numbered lists for steps and tables for comparisons.
- **Understand.** Use words the reader already knows. Define each new term where it first appears, and keep using that term.
- **Use.** Order steps as the reader will do them, one action per step. After a step, say what the reader should see. End when the reader has what they need.

## Pass 2: Order the paragraphs (Williams)

Joseph Williams' *Style: Lessons in Clarity and Grace* shows that readers follow a paragraph when each sentence starts with something they know.

- **Put old information before new.** Open a sentence with what the previous sentence or the context already gave. Close it with what is new. That new idea then opens the next sentence.
- **Put the weight at the end.** Readers stress the last words of a sentence. Save that position for the important idea, and move qualifiers like "in most cases" earlier.
- **Keep the same subjects.** Across a paragraph, let the subjects name the same few characters. When the subject keeps changing, readers lose the thread.
- **State the point early.** The first or second sentence of a paragraph says what the paragraph is for.

## Pass 3: Fix the sentences (Strunk and White)

- **One idea per sentence.** Length follows the idea, so a long sentence is fine when its idea needs the room. Split a sentence that carries two ideas.
- **Make the actor the subject and the action the verb.** "Validation of the input is performed by the parser" becomes "The parser validates the input."
- **Prefer the active voice.** Use the passive only when the actor is unknown or does not matter.
- **State things positively.** Write "forgot" for "did not remember" and "late" for "not on time".
- **Be specific.** "The build fails on Node 18" tells the reader more than "There may be compatibility concerns."
- **Cut words that do no work.** "In order to" becomes "to", and "at this point in time" becomes "now".
- **Give parallel ideas parallel grammar,** especially in lists and headings.
- **Reach the main verb early.** Readers hold a long subject in memory until its verb arrives.

## Pass 4: Choose the words (Garner)

Bryan Garner's *Modern English Usage* records the forms careful writers use today. Follow it when a usage is in doubt.

- **Use the plain word.** Write "use" for "utilize", "about" for "with regard to", "before" for "prior to" and "help" for "facilitate".
- **Keep confusable pairs straight,** such as affect and effect, comprise and compose, fewer and less, imply and infer.
- **Avoid words whose meaning is disputed,** such as "decimate", or "hopefully" meaning "I hope". Whichever sense you intend distracts some readers.
- **Cut redundant phrases** such as "end result", "future plans" and "completely eliminate".
- **Cut intensifiers and hedges** such as "very", "really", "basically", "simply" and "just".
- **Call one thing by one name.** A reader who meets "workspace" and later "project" assumes they are two different things.
- **Use the reader's words** in place of internal names and code names.

## Last check: read as the reader

Read the draft as the reader you named. If they cannot find the answer within ten seconds, move it up. If they would need to ask you a question before acting, answer it in the text.

## Writing requirements (RFC 2119)

Specs, policies and agent instructions mark their requirements with the RFC 2119 keywords. RFC 8174 adds that the keywords carry this meaning only in uppercase. In lowercase, "must" is ordinary English.

| Keyword | Meaning |
|---|---|
| MUST, REQUIRED, SHALL | The reader has to do it |
| MUST NOT, SHALL NOT | The reader may never do it |
| SHOULD, RECOMMENDED | The reader does it unless they have a good reason and accept the cost |
| SHOULD NOT, NOT RECOMMENDED | The reader avoids it unless they have a good reason and accept the cost |
| MAY, OPTIONAL | The reader chooses freely |

- **Give the reason** behind any requirement whose reason is not obvious. A reader who knows the reason can apply the rule to cases you did not foresee.
- **Use the keywords sparingly.** When every line says MUST, no line stands out.
- **Declare them in formal specs.** Near the top, write: "The key words MUST, MUST NOT, SHOULD, SHOULD NOT and MAY are to be read as described in RFC 2119 and RFC 8174."
- **Keep them out of marketing and conversation.**

## Editing someone else's text

Keep the author's voice and meaning. Change what is unclear, and leave what only differs from how you would write it.

## Other rules come first

The user's own style rules override this skill.
