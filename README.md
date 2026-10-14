# Brand Discovery Interview

A reusable agent skill for interviewing founders about brand purpose, vision, positioning, voice and social content. It asks one question at a time, keeps evidence separate from aspiration, and can reconcile independent founder interviews without hiding disagreements.

**Status:** Initial release. Validation scope and remaining limitations are documented in [VALIDATION.md](VALIDATION.md). The default is 100 main questions; that count is configurable and is not a research-validated quality threshold.

## Contents

```text
skills/brand-discovery-interview/
  SKILL.md
  agents/openai.yaml
  references/interview-and-checkpoints.md
  references/guide-and-reconciliation.md
examples/onyx-cofounder-prompt.md
```

The skill has no required external tool, model council, API key or Python dependency. Optional source verification and external review require actual connected, authorised tools. The ONYX example is a copy-paste prompt with that business's chosen constraints; those constraints are not the general skill's defaults.

## Use it

Place the entire `skills/brand-discovery-interview` folder in a supported skill location. For a Codex repository, use `.agents/skills/brand-discovery-interview`; for other hosts, follow their skill-import instructions. This repository is source, not a published plugin-directory listing.

Start:

```text
Use $brand-discovery-interview to interview me about Example Studio.
Ask 100 main questions, one question at a time. Label me Founder A.
```

Resume:

```text
Use $brand-discovery-interview to resume my Example Studio interview.
Here is my saved checkpoint and any newer replies:
[paste the actual checkpoint and replies]
```

Request an early guide:

```text
Use $brand-discovery-interview to synthesize a provisional guide from the
answers currently available. Show the question counts and evidence gaps.
```

Combine independent founder perspectives:

```text
Use $brand-discovery-interview to reconcile the two supplied founder reports.
Compare by theme, preserve material disagreements and propose decisions for us.
Do not claim we have approved a combined identity.
```

If your host does not import skills, you can use the [ONYX example prompt](examples/onyx-cofounder-prompt.md) in an ordinary chat after adapting the brand and business-specific rules.

## Configuration and records

Supply the brand, participant label, preferred question count and relevant media/approval policies. Only the brand is needed before the interview can begin; other missing choices use stated defaults or are discovered during the interview.

Save every checkpoint outside the chat. A checkpoint can support continuation; a complete verbatim archive still needs the original transcript blocks. Keep founders' discovery interviews independent until each is ready for comparison. The output remains provisional pending founder decisions and customer validation.

Do not commit real interview answers, customer records or private checkpoints to a public repository without appropriate authorisation. This package includes no real interview answers.

## Sources and scope

Skill packaging follows [OpenAI's skill documentation](https://learn.chatgpt.com/docs/build-skills). The interview workflow is a custom synthesis, not an official Ruben Hassid, StoryBrand or Nielsen Norman Group product. It makes no claim that a 100-question interview has been shown to outperform other discovery methods.

## License

MIT. See [LICENSE](LICENSE).
