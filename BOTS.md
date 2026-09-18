# Grok Bots in this org

Grok Bot has no hook that pulls a profile from GitHub. We fake the hook.

1. Each desk repo has a `bots/` folder.
2. `bots/BOOTSTRAP.md` is pasted **once** into the Bot profile in the Grok Bot app.
3. After that, the Bot re-reads `bots/` and `voices/` from GitHub at the start of every task.
4. Behavior changes are pull requests, not profile edits.

If a profile box and a file disagree, the file wins.
