# UX Architect & Usability Critic

An agent skill for reviewing product navigation, information architecture, feature placement, and user journeys.

**Reduce confusion, not merely clicks.**

Use it to question where functionality belongs, make terminology consistent, improve discovery, and design complete interactions. Review depth scales with the decision: a label fix should not become a product-wide redesign.

## Install in Codex

Clone the repository and copy the skill folder into your project:

```sh
git clone https://github.com/SscSPs/ux-architect.git
mkdir -p /path/to/your-project/.agents/skills
cp -R ux-architect/skills/ux-architect /path/to/your-project/.agents/skills/
```

For use across projects, copy it into `~/.agents/skills/` instead. Start a new Codex session after installation. See the [skill source](skills/ux-architect/SKILL.md) for the complete instructions.

## Use

Invoke `$ux-architect` and give the agent access to the relevant product context.

### Review

> Use $ux-architect to review where recurring transactions belong in this app. Inspect the current navigation and related transaction flows. Report findings and recommendations; do not edit files.

### Design

> Use $ux-architect to propose a clearer account setup flow. Consider new users, recovery from errors, and conventions already used elsewhere. Explain meaningful trade-offs without implementing changes.

### Implement

> Use $ux-architect to improve discoverability of transaction filters. Inspect comparable controls, make the smallest coherent change, and preserve unrelated behavior. Follow this project's verification instructions and report what was actually verified.

## What to expect

- User goals and observable success criteria before material changes.
- Scope proportional to the decision and consistency with related features.
- Accessibility, recovery paths, and migration costs considered where relevant.
- Evidence separated from assumptions, and impact separated from confidence and effort.
- Reviews produce recommendations; implementation requests authorize changes within their scope.

## Limits

This is a UX reasoning skill, not a visual design system. Architecture-level recommendations need navigation, related workflows, terminology, and product requirements; a single component rarely provides enough context.

Hypothetical walkthroughs are not user research. The skill does not establish accessibility compliance or guarantee usability improvements. This initial release has not been behaviorally evaluated against real user tasks.

## Contributing

Report concrete failures with the task, relevant context, expected behavior, and actual output. Remove private product data before sharing examples. Prefer corrections supported by observed behavior over additional general rules.

## License

MIT — see [LICENSE](LICENSE).
