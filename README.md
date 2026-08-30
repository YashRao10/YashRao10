# Yash Rao

Solutions Engineer at HummingBird Technosys, working on a DO-178C / DO-254 / DO-278A
compliance platform for aerospace software certification. B.S. in Technology and
Information Management, minor in Economics, UC Santa Cruz.

I work at the point where AI tooling meets safety-critical software assurance: what it
takes to actually trust an AI agent inside a regulated process, and how you show it.

## Selected work

**[mcp-ratchet](https://github.com/YashRao10/mcp-ratchet)** is a security scanner and
runtime drift monitor for MCP servers. Existing scanners check a server once at install.
This one fingerprints a server's tool surface and keeps checking it against that baseline,
so a post-approval change (a "rug pull") produces a drift event instead of going unnoticed.
Static checks cover injected instructions, permission mismatches, secrets, and dependency
CVEs. Live dashboard tracking 5 real servers, 195 tests.

**[DO-330 tool qualification study](https://github.com/YashRao10/mcp-ratchet/tree/main/qualification)**
is a full worked example of taking mcp-ratchet's deterministic drift-detection function
through DO-330: the qualification trigger, eleven Tool Operational Requirements, verification
cases, and an honest verdict (candidate TQL-5 under Criteria 3, for a bounded use). Writing
the requirements against the source turned up three real defects in the tool. A cold
independent reviewer re-ran the verification. There is very little public material on
qualifying anything in an AI toolchain under DO-330.

**[AI Compliance Crosswalk](https://github.com/YashRao10/ai-compliance-crosswalk)** assesses
three real AI agents running on my own machine, control by control, against every substantive
EU AI Act high-risk requirement and all four NIST AI RMF functions. Each verdict is grounded
in real evidence (system prompts, red-team history, governance notes), reached by reading
each control rather than keyword-matching or scoring it with a script.

**[YR Signal](https://yashrao10.github.io/signal-log/)** is a public trade log and market and
economic research site: every trade with its reasoning, plus a regime classifier, a
synthetic-control event-study toolkit, a GDP bridge-equation nowcast, and factor
decomposition. No position sizes, only the thinking.

**[GPT From Scratch](https://github.com/YashRao10/gpt-from-scratch)** is a decoder-only
transformer built from first principles in PyTorch: manual causal self-attention, a
from-scratch byte-level BPE tokenizer, KV-cache. A learning project, logged honestly. Stage 5
found real underfitting and I wrote that up rather than bury it.

## Elsewhere

- Portfolio hub: [yashrao10.github.io](https://yashrao10.github.io)
- LinkedIn: [yash-r-84866a171](https://www.linkedin.com/in/yash-r-84866a171/)
