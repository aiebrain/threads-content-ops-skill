# Threads Content Ops Skill

A public, shareable Hermes skill for running a Threads-style content operation with a **human approval gate**.

This is not an auto-spam or bulk-posting system. It is a repeatable content operations workflow for creators, educators, and solo operators who want to treat short-form social content as a small operating system.

```text
research / account performance check
→ draft candidates
→ human approval
→ approved-only publishing
→ live post verification
→ comment / DM analysis
→ next-post adjustment
→ operating log
```

## Why this exists

Many content workflows stop here:

```text
idea
→ write
→ publish
→ done
```

That creates a reset problem. Every post starts from scratch, comments are not converted into future ideas, and publishing may happen without a clear approval or verification step.

This skill turns social posting into a feedback loop:

```text
write
→ approve
→ publish
→ verify
→ learn
→ adjust the next post
```

## What the skill does

The skill helps an agent run this loop:

1. Review current context and prior performance.
2. Compare against public benchmark post structures.
3. Choose one business or conversion route.
4. Draft multiple candidate posts.
5. Wait for explicit human approval.
6. Publish only approved posts.
7. Verify the live post and all reply segments.
8. Analyze comments, DMs, and response quality.
9. Adjust the next post based on evidence.
10. Record the operating log.

## Core operating model

### 1. Research and performance check

Before drafting, review three lenses:

| Lens | What to check |
|---|---|
| External benchmark | Hook, contrast, CTA, post length, reply structure |
| Own-account signal | Views, useful comments, saves/shares, repeated questions |
| Business route | Comment, DM, resource request, consultation, product/service question |

The point is not to copy viral posts. Extract the structure only.

### 2. Candidate drafting

Do not jump to one final post too quickly. Prepare multiple candidates and make them different.

Each candidate should include:

```text
candidate number
title
style
purpose
business route
expected success signal
benchmark shape
approval CTA
main post
author reply / expansion reply
```

Useful style rotation:

- short insight
- problem diagnosis
- real work example
- checklist
- contrarian statement
- conversational diary
- comment prompt
- mini story
- before/after
- beginner mini lesson

### 3. Human approval gate

Drafting is not publishing.

Examples of acceptable approvals:

```text
Candidate 1 approved
Publish the first one now
Approve all three
Publish candidate 1; adjust the others after results
```

Rules:

- Never publish before explicit approval.
- Publish only approved posts.
- If later posts depend on earlier results, do not finalize them too early.

### 4. Publishing structure

For multi-part Threads, split content into segments.

Example:

```text
1/3 main problem or insight
2/3 example or explanation
3/3 concrete CTA or question
```

Before publishing, prepare sentinel phrases for verification:

```json
{
  "segments": [
    "main post text",
    "author reply text",
    "CTA reply text"
  ],
  "sentinels": [
    "unique phrase from main post",
    "unique phrase from author reply",
    "unique phrase from CTA reply"
  ]
}
```

### 5. Live verification

Publishing is not complete when the button is clicked.

Verify:

- new canonical URL exists
- feed/profile shows the new hook
- expected `1/N` reply structure appears
- hidden replies are expanded if needed
- final CTA appears
- no missing or duplicated tail segment exists

Do not rely only on a returned URL or a clicked publish button.

### 6. Comment and DM analysis

Use this priority order:

```text
qualified contact / DM / problem statement
> product or service question
> useful comment
> save/share
> follow
> views
```

A useful comment is not just engagement. It can become the next post.

Example:

```text
comment question
→ short clarification reply
→ beginner-friendly follow-up post if the question repeats
```

### 7. Result-based adjustment

Adjust the next post based on the first result.

| Situation | Adjustment |
|---|---|
| Strong response | Expand the same theme |
| Views but no comments | Make the CTA more concrete |
| Replies are not read | Move more substance into the main post |
| Basic question appears | Create a beginner follow-up |
| DMs or product questions appear | Route toward the relevant resource, offer, or conversation |

## Install into Hermes

Clone this repository:

```bash
git clone https://github.com/aiebrain/threads-content-ops-skill.git
```

Copy the skill into your Hermes skills directory:

```bash
mkdir -p ~/.hermes/skills/social-media
cp -R threads-content-ops-skill/skills/social-media/threads-content-ops ~/.hermes/skills/social-media/
```

Verify:

```bash
hermes skills list | grep threads-content-ops
```

Or load it inside Hermes:

```text
skill_view(name="threads-content-ops")
```

## Package contents

```text
README.md
LICENSE
skills/social-media/threads-content-ops/SKILL.md
skills/social-media/threads-content-ops/references/public-workflow.md
skills/social-media/threads-content-ops/templates/daily-approval-request.md
skills/social-media/threads-content-ops/templates/publish-log.md
```

## Templates

### Daily approval request

Use:

```text
skills/social-media/threads-content-ops/templates/daily-approval-request.md
```

This template structures a daily approval message with three candidates, selection basis, business route, expected success signal, and approval options.

### Publish log

Use:

```text
skills/social-media/threads-content-ops/templates/publish-log.md
```

This template records approval, publish time, canonical URL, segment verification, visible metrics, useful comments, and next-post adjustment.

## Public distribution record

```text
Repository: aiebrain/threads-content-ops-skill
URL: https://github.com/aiebrain/threads-content-ops-skill
Visibility: PUBLIC
Default branch: main
Initial public commit: 537d315 Add public Threads content ops skill
```

## Public safety checklist

Before sharing or adapting this workflow, remove or generalize:

- personal local paths
- private channel IDs
- browser profile names
- internal automation endpoints
- private account operations
- API keys, tokens, cookies, and passwords
- customer, student, or client data
- unpublished business strategy

## Safety principles

- Keep a human approval gate before publishing.
- Do not publish private or sensitive information.
- Do not store access tokens, cookies, API keys, or passwords in logs.
- Use browser automation only with your own account or a properly authorized account.
- Verify live posts after publishing.
- Use public-safe examples when sharing this workflow externally.

## One-line summary

```text
Threads operations are not about writing more posts; they are about recording response signals and adjusting the next post.
```

## License

MIT
