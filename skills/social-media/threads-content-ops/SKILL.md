---
name: threads-content-ops
description: "Use when running a human-approved Threads content operation: performance review, draft candidates, approval gate, browser-based publishing, live verification, comments/DM analysis, and next-post adjustment."
---

# threads-content-ops

Use this skill when a creator or business account needs a repeatable Threads-style content operation with a human approval gate.

This is a public-safe workflow skill. It does not assume a specific account, private system, local path, token, or browser profile.

## Core loop

```text
1. Review context and prior performance
2. Choose a business/conversion route
3. Draft multiple post candidates
4. Ask the human to approve one or more candidates
5. Publish only approved posts
6. Verify the live post and all reply segments
7. Analyze comments, DMs, and response quality
8. Adjust the next post
9. Record the operating log
```

## When to use

Use this for requests like:

- `Plan today's Threads posts`
- `Analyze yesterday's Threads result and adjust today's posts`
- `Draft three candidates for approval`
- `Publish candidate 1 after approval`
- `Write a reply to this comment`
- `Turn this content workflow into a repeatable operating system`

## Companion capabilities

Pair this skill with:

- a content/copywriting skill for writing candidates
- browser automation when publishing through a logged-in browser
- a note-taking or knowledge-base workflow for operating logs
- a social research workflow when benchmarking external post shapes

## Drafting lens

Before writing, resolve these three lenses.

### 1. External benchmark lens

Extract only the structure from public high-signal posts:

- hook shape
- contrast or before/after
- proof/output
- CTA style
- thread length
- whether replies expand the idea or repeat it

Do not copy the original wording.

### 2. Own-account performance lens

Use recent posts to identify what already works:

- views
- likes/replies
- saves/shares where visible
- comments and questions
- which topics or formats produced useful conversations

If metrics are incomplete, label the limitation and use visible evidence only.

### 3. Business route lens

Every post should have one primary next action, such as:

- comment with a problem
- DM for a resource
- save a checklist
- ask a product/service question
- join a challenge or newsletter
- book a consultation

Metric priority:

```text
qualified contact / DM / problem statement
> product or service question
> useful comment
> save/share
> follow
> views
```

## Candidate format

When preparing daily candidates, use different styles rather than repeating one format.

For each candidate, include:

```text
candidate number
working title
style
purpose
business route
expected success signal
benchmark shape
approval CTA
main post
author reply / expansion reply
```

Style bank:

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

## Approval gate

Never publish without explicit human approval.

Accepted approvals can look like:

```text
Candidate 1 approved
Publish the first one now
Approve all three
Publish only candidate 1; adjust 2 and 3 after results
```

Rules:

- Draft generation is not publication.
- Publish only approved posts.
- If later posts depend on earlier results, do not finalize them too early.

## Publishing preparation

For multi-part Threads, prepare segments and verification sentinels before publishing.

Example:

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

## Live verification checklist

After publishing, verify:

1. A new canonical post URL exists.
2. The profile/feed shows the new hook.
3. The expected thread count appears, such as `1/3`, `2/3`, `3/3`.
4. Hidden replies are expanded.
5. Every sentinel phrase appears.
6. The final CTA or conversion reply is present.

Do not rely only on a returned URL or a clicked publish button.

## Comment reply style

When replying to comments:

- Be short.
- Answer the exact misunderstanding first.
- Avoid over-explaining.
- Use the question as a possible next-post angle.
- Give one recommended reply unless the user asks for options.

Template:

```text
Good question.
In this post, I mean [simple clarification].
So the difference is [A] vs [B].
```

## Result-based adjustment

After 1–2 hours, inspect the post if possible.

Adjust like this:

- Good response → expand the same theme in the next post.
- Views but no comments → make the CTA more concrete.
- Replies are not read → move more substance into the main post.
- A basic question appears → answer simply and create a beginner-friendly follow-up post.
- DMs or product questions appear → route to the appropriate resource, offer, or conversation.

## Operating log

Record:

- date/time
- candidate plan
- approval decision
- published URL
- segment verification
- visible metrics
- useful comments/questions
- adjustment decision for the next post

Use the template in `templates/publish-log.md`.
