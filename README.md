# Technical AI Evaluation for Legal, Compliance & Risk Management Teams

Training content for an 8-hour programme for AXA, delivered in two virtual sessions of 4 hours each. The programme teaches non-technical reviewers how to look at an AI proposal and say how it works, where data goes, what can go wrong, what to ask the vendor and what proof to request.

Trainer: Ramanuj Das.

## Who it is for

Legal, Compliance and Risk Management professionals who review AI tools but do not build them. No technical background is assumed.

Every exercise shows two views of the same finding:

- **Legal & Compliance:** Is it allowed? Is it in the contract? Were people told? Who is accountable?
- **Risk Management:** What could happen? How likely? How bad? What controls exist, and what risk is left?

## Programme at a glance

### Session 1: How AI actually works

| Block | Topic | Participant files |
| --- | --- | --- |
| 0 | Welcome | [welcome-intro.md](content/session-1/welcome-intro.md) |
| 1 | The AI family | [explainer](content/session-1/b1-ai-family/explainer.md), [hands-on](content/session-1/b1-ai-family/handson.md) |
| 2 | How an LLM works | [explainer](content/session-1/b2-how-llm-works/explainer.md), [hands-on](content/session-1/b2-how-llm-works/handson.md) |
| 3 | Chat app vs agent | [explainer](content/session-1/b3-chat-vs-agent/explainer.md), [hands-on](content/session-1/b3-chat-vs-agent/handson.md) |
| 4 | The complete flow | [explainer](content/session-1/b4-complete-flow/explainer.md), [hands-on](content/session-1/b4-complete-flow/handson.md), [RAG explainer](content/session-1/b4-complete-flow/rag-explainer.md), [RAG hands-on](content/session-1/b4-complete-flow/rag-handson.md) |

### Session 2: How to check an AI tool

| Block | Topic | Participant files |
| --- | --- | --- |
| 5 | What can go wrong | [explainer](content/session-2/b5-what-can-go-wrong/explainer.md), [hands-on](content/session-2/b5-what-can-go-wrong/handson.md), [key risk areas](content/session-2/b5-what-can-go-wrong/key-risk-areas.md), [key risk areas hands-on](content/session-2/b5-what-can-go-wrong/key-risk-areas-handson.md) |
| 6 | Rules into questions; promise vs proof | [explainer](content/session-2/b6-rules-to-questions/explainer.md), [hands-on](content/session-2/b6-rules-to-questions/handson.md), [requirements to controls](content/session-2/b6-rules-to-questions/requirements-to-controls.md), [requirements hands-on](content/session-2/b6-rules-to-questions/requirements-handson.md) |
| 7 | Guardrails | [explainer](content/session-2/b7-guardrails/explainer.md), [hands-on](content/session-2/b7-guardrails/handson.md) |
| 8 | Capstone: review the UW Copilot proposal | Not written yet |

Sample documents used in the hands-on exercises sit in a `documents/` folder inside each block.

## Repository layout

```text
CLAUDE.md          Instructions for generating content with Claude Code
content/           Participant material: explainers, hands-on sheets, sample documents
  session-1/       Blocks 1 to 4
  session-2/       Blocks 5 to 8
trainer-only/      Demo scripts, answer keys, trainer notes, session plan (not in the repository)
```

## Trainer-only material

Answer keys, demo scripts, trainer notes and the minute-by-minute session plan are kept in `trainer-only/`. That folder is listed in `.gitignore`, so it is never committed or shared. Do not move trainer material into `content/`: participant files must never contain answers.

## Conventions

- **File header.** Every file starts with a front-matter block: title, session, block, type, duration and audience.
- **Duration.** The `duration` in a header is the time that file gets on the agenda. For a hands-on, it includes the trainer's briefing and debrief.
- **File types.** `explainer.md`, `handson.md`, `handson-answers.md`, `demo-script.md`, `quiz.md` and `trainer-notes.md`. Names are lowercase, with hyphens.
- **Running case.** ClaimAssist, a fictional claims assistant from the fictional vendor Nimbus AI Solutions Ltd, grows through three versions: chat, chat with documents, and agent. Its fixed facts are listed in [CLAUDE.md](CLAUDE.md) and must not be contradicted.
- **Style.** Plain British English, short sentences, one everyday analogy per idea. No emojis, and no code in participant files.
- **Diagrams.** Mermaid, using the colour classes defined in [CLAUDE.md](CLAUDE.md). They render on GitHub, and in VS Code with the Markdown Preview Mermaid Support extension.

## Adding or changing content

[CLAUDE.md](CLAUDE.md) is the full brief: audience, programme structure, the eight-step flow, the six risks, templates for each file type, diagram rules and a quality checklist. Read it before writing anything new. If you use Claude Code in this folder, it follows that brief automatically. For example:

```text
Create the explainer and hands-on for Session 2, Block 8 (capstone).
```

After any change, check that the header duration still matches the timing table in the matching answer key and the slot in the session plan.

## Still to write

- Block 8 capstone: the UW Copilot proposal, the hands-on sheet and the answer key.
- Shared files in `content/00-shared/`: the ClaimAssist case, glossary and evaluation checklist.
- Demo scripts for Blocks 2, 4, 6 and 7.
- Quizzes.

## Data and scope

- All people, companies, policies, claims and vendors are fictional. Sample documents are marked "Fictional - for training only".
- Never enter real company, customer or personal data into Copilot, Ollama or any other tool, in preparation or in a session.
- The programme frames questions and proof requests. It does not give legal or regulatory interpretation.
