# AGENTS.md

Instructions for coding agents in this repository. They bind every change.

pulse-agent is the Linux host agent of pulse, written in Rust; see `README.md`. Work arrives as an issue with an approved spec from the meta repository; implement only the section for this repository.

## Code conventions

The pulse [code conventions](https://github.com/lorenzh/pulse-meta/blob/main/docs/code-conventions.md) apply to every change. Search the crate for an existing function or module before writing one, and move the second copy of a pattern into a shared one. Keep metric parsing and formatting in small pure functions; reading the host and sending to pulse-api stay at the edge.
