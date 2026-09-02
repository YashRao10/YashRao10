# Yash Rao

Customer-focused Technology and Information Management graduate with ability to bridge technical solutions with business strategy through solid understanding of information systems and economic principles. Passionate about communicating the value of technology in order to satisfy customer needs.

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

### [dal-c](https://github.com/YashRao10/dal-c)

15 small C components written the way avionics software is, following DO-178C at Design
Assurance Level C. Every component has a requirements doc, the code is tagged back to each
requirement, and the tests have to cover every function to 100 percent MC/DC or CI won't
pass. No malloc, no recursion. Right now that is 73 high-level and 182 low-level
requirements, 2479 test checks, and a fuzz run of 200,000 iterations that stays clean under
the sanitizers and on gcc, clang and 32-bit. The [site](https://yashrao10.github.io/dal-c/)
rebuilds the traceability matrix and coverage report from each run, so what it shows is
always current.

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
