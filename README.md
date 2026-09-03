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

### [DO-330 tool qualification study](https://github.com/YashRao10/mcp-ratchet-do330)

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

## Markets and economics

### [Causal Toolkit](https://github.com/YashRao10/causal-toolkit)

A synthetic-control research instrument. Point it at any market or company event and any
ticker, and it runs the Abadie-Diamond-Hainmueller synthetic-control method to test whether
the event actually caused a break from a hand-picked peer group, or whether the move is just
a pre-existing trend or estimation noise. Each run writes a self-contained HTML report with
an actual-vs-synthetic chart, placebo tests, and a written verdict, and regenerates a
browsable index of every case run so far.

### [FRED Nowcast](https://github.com/YashRao10/fred-nowcast)

A small, transparent GDP nowcasting model. It predicts real GDP growth from five
higher-frequency FRED indicators (industrial production, retail sales, initial claims,
payrolls, housing starts) with a plain OLS bridge equation, and checks itself against a
naive baseline with an honest walk-forward backtest before claiming it is worth anything.

### [Regime Classifier](https://github.com/YashRao10/regime-classifier)

Classifies market history into six named macro regimes from FRED data (the yield curve, the
Fed funds path, inflation, unemployment), then backtests how all 11 GICS sector ETFs plus
gold and long Treasuries have performed in each regime since 1999. It turns an ad hoc "what
is the Fed backdrop doing to these sectors" question into a re-runnable one. The taxonomy is
a rule set I built for the project, and the README says so plainly.

## Elsewhere

- Portfolio hub: [yashrao10.github.io](https://yashrao10.github.io) (YR Hub, links every
  live tool and finished project in one place)
- LinkedIn: [yash-r-84866a171](https://www.linkedin.com/in/yash-r-84866a171/)
