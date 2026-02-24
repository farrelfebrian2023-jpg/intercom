# Proof Artifacts

Run date: 2026-02-24 16:05:29 +07:00

Fork: https://github.com/farrelfebrian2023-jpg/intercom
Custom app label: Intercom Agent Handoff Ledger
Namespace slug: intercom_core
Mutating command: seal_agent_handoff_intercom_core
Query command: inspect_agent_handoff_intercom_core
Payout Trac address: trac1tuhvnnxnrng36vdtn8en9004nu6544c7s4fj3cvmk3nwrk6f83pq2n2xxe

Naming rationale:
- Domain noun uses `agent_handoff` to represent handoff status tracking between operators and agents.
- Namespace suffix `intercom_core` keeps this fork naming isolated without embedding username.
- Verb pair `seal` (mutating) and `inspect` (query) separates write/read intent clearly.

Included files:
- `run.log`: sanitized runtime log from `pear run` proof session.
- `run-screenshot.png`: image generated from top section of `run.log`.
- `command-mapping.log`: direct output of protocol command mapping checks.
- `tx-sim.log`: runtime `cli_result` capture for `/tx --command ... --sim 1` via SC-Bridge CLI.

Runtime tx simulation commands:
- `/tx --command '{"op":"seal_agent_handoff_intercom_core","status":"MVP ready","note":"first demo"}' --sim 1`
- `/tx --command "inspect_agent_handoff_intercom_core" --sim 1`

