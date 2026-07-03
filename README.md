# Threads Content Ops Skill

A shareable Hermes skill for running a Threads-style content operation with a human approval gate.

This package is for creators, educators, and solo operators who want a repeatable workflow for:

```text
research / account performance check
→ draft candidates
→ human approval
→ browser-based publishing
→ live post verification
→ comment / DM analysis
→ next-post adjustment
→ operating log
```

## What this is

This is not an auto-spam or bulk-posting system. It is a **human-in-the-loop content operations workflow**.

The core idea is simple:

1. Draft multiple post candidates from evidence.
2. Let a human approve what actually gets published.
3. Publish only approved posts.
4. Verify that the live post exists and all reply segments are present.
5. Use the result to adjust the next post.

## Install into Hermes

Copy the skill folder into your Hermes skills directory:

```bash
mkdir -p ~/.hermes/skills/social-media
cp -R skills/social-media/threads-content-ops ~/.hermes/skills/social-media/
```

Then verify:

```bash
hermes skills list | grep threads-content-ops
```

## Contents

```text
skills/social-media/threads-content-ops/SKILL.md
skills/social-media/threads-content-ops/references/public-workflow.md
skills/social-media/threads-content-ops/templates/daily-approval-request.md
skills/social-media/threads-content-ops/templates/publish-log.md
```

## Safety principles

- Keep a human approval gate before publishing.
- Do not publish private or sensitive information.
- Do not store access tokens, cookies, API keys, or passwords in logs.
- Verify live posts after publishing.
- Use public-safe examples when sharing this workflow externally.

## License

MIT
