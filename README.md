# Yash Rao

Solutions Engineer at HummingBird Technosys, working on a DO-178C / DO-254 / DO-278A
compliance platform for aerospace software certification. B.S. in Technology and
Information Management, minor in Economics, UC Santa Cruz.

I work at the point where AI tooling meets safety-critical software assurance: what it
takes to actually trust an AI agent inside a regulated process, and how you show it.

## Selected work

### [MCP Server Security (mcp-ratchet)](https://github.com/YashRao10/mcp-ratchet)

A security scanner and runtime drift monitor for MCP (Model Context Protocol) servers.
Existing scanners check a server once at install time; mcp-ratchet fingerprints a server's
tool surface and keeps checking it against that baseline, so a tool definition that
silently changes after a person approved it gets caught. One judgment check runs through a
real Claude API call to flag prompt-injection language in tool descriptions; the rest are
deterministic checks for permission mismatches, exposed secrets, and pinned-dependency
CVEs, and every finding is labeled by which source produced it. Live dashboard tracks 5
real public servers. 195 tests, fully open source.

### [DO-330 tool qualification study](https://github.com/YashRao10/mcp-ratchet/tree/main/qualification)

A full worked example of taking mcp-ratchet's deterministic drift-detection function
through DO-330: the qualification trigger, eleven Tool Operational Requirements,
verification cases, and an honest verdict (candidate TQL-5 under Criteria 3, for a bounded
use). Writing the requirements against the source turned up three real defects in the tool,
and a cold independent reviewer re-ran the verification. There is very little public
material on qualifying anything in an AI toolchain under DO-330.

### [AI Compliance Crosswalk](https://github.com/YashRao10/ai-compliance-crosswalk)

A compliance crosswalk tool mapping the EU AI Act and NIST AI RMF requirements to real
evidence for real AI agents. The verdicts are written in session against actual evidence
and not scored by a script. It includes a remediation tracker, an automated deploy
pipeline, and 35 passing tests.

### [YR Signal](https://yashrao10.github.io/signal-log/)

Designed and built a public markets research and trade transparency site that I maintain
myself. It includes sanitized trade history with written thesis notes, sector performance
visualizations, and live macroeconomic data. I handled the full stack from the design
system to the data pipeline to deployment, and kept one strict privacy rule in place
throughout: no dollar amounts or position sizes are shown, anywhere.

### [GPT From Scratch](https://github.com/YashRao10/gpt-from-scratch)

Built a GPT-style decoder-only transformer from scratch in PyTorch: custom tokenizer,
causal self-attention, and autoregressive sampling, with no pretrained weights or
high-level libraries. Ran a series of training experiments varying model size and
learning-rate schedule, cutting validation loss from 1.75 to 1.62 across the runs.

## Elsewhere

- Portfolio hub: [yashrao10.github.io](https://yashrao10.github.io) (YR Hub, links every
  live tool and finished project in one place)
- LinkedIn: [yash-r-84866a171](https://www.linkedin.com/in/yash-r-84866a171/)
