# Agent Handoff Kit

[中文](README.md) · English

Markdown templates for handing a task to another AI assistant with its materials, current decisions, next action, acceptance criteria, and return destination.

**[Download v0.1.0 ZIP](https://github.com/arden-workroom/agent-handoff-kit/releases/download/v0.1.0/agent-handoff-kit-v0.1.0.zip) · [Give feedback](https://github.com/arden-workroom/agent-handoff-kit/issues/new/choose)**

This is a manual document kit: four templates, a receiver prompt, and fictional worked examples. No software installation is needed. You use your own AI service and its normal pricing.

## Try one complete handoff

Copy this entire block into the AI assistant receiving the task. It contains all the material needed for the example.

```text
Take over this writing task. Read all the material below and deliver the actual revision.

Goal and scope: make a creative tool description clear to a reader with no technical background. Rewrite only paragraphs 1 and 2. Preserve paragraph 3 exactly.

Draft:
1. This tool uses multimodal semantic aggregation and cross-stage knowledge orchestration to build a cognitive collaboration system from inspiration input to artifact output.
2. Users can apply structured information containers, dynamic routing strategies, and feedback loops to optimize personal creative activity.
3. Start by saving one idea, then choose writing, images, or research.

Product facts you may use:
Users can record ideas, choose a creative direction, add relevant material, see the next step, and leave revision feedback. Abstract wording in the draft is not evidence of additional features.

Decisions:
D-001, superseded: make the whole text sound professional by adding jargon.
D-002, current: use familiar words for nontechnical readers. This replaces the style requirement in D-001.
D-003, current: rewrite only paragraphs 1 and 2; preserve paragraph 3 exactly.

Return all three paragraphs, followed by two sentences explaining the changes to the first two. Do not invent features, performance numbers, or promises. Return the result in this conversation for review. No external sending or publishing is requested.
```

Check the result:

- It contains three paragraphs and two explanatory sentences.
- The first two paragraphs follow D-002, rather than the superseded instruction.
- The final paragraph is exactly: `Start by saving one idea, then choose writing, images, or research.`
- It stays within the supplied product facts.

This is a fictional teaching example, not an independent evaluation of a model. The detailed Chinese walkthrough and a possible output are in [example one](examples/01-writing/START_HERE.md).

## Adapt a small task

```text
Goal:
Material: paste the relevant text or attach files the receiver can actually open.
Current decision: what applies now, and which earlier instruction it replaces.
Next action: the specific step to complete this time.
Acceptance criteria: what to deliver and what to preserve.
Return destination: where the result goes, who reviews it, and how to continue.
```

For a larger task, use the [handoff template](templates/handoff.md), [decision log](templates/decisions.md), [return note](templates/return.md), and [review checklist](templates/review.md). These detailed templates are currently in Chinese. This page provides an English quickstart and minimal handoff card.

When evidence is missing, distinguish useful partial work from unsupported conclusions. The [second worked example](examples/02-missing-evidence/START_HERE.md) demonstrates this using a task with no audio material.

## Scope and evidence

The kit does not run a backend, call model APIs, execute tasks automatically, share memory, or connect accounts. Passing a template does not grant access or permission to act in another service.

The fixtures and sample outputs were authored and reviewed by the same AI. External user testing and independent model evaluation have not been completed. No time-saving or success-rate results are claimed. See the [validation record](docs/scope-and-validation.md).

## Privacy and feedback

Sending task materials to an AI sends them to that service. Share only what the task needs and what you are allowed to disclose.

[Report a confusing step or suggest a change](https://github.com/arden-workroom/agent-handoff-kit/issues/new/choose). Use a fictional or public example. Remove private contact details, credentials, private conversations, and private file links. See [contributing](CONTRIBUTING.md) for maintenance expectations.

## License

[MIT](LICENSE). Commercial use, modification, and redistribution are permitted, subject to preserving the copyright and license notice.

Maintained by **Arden**.
