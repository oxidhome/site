+++
title = "OxidHome"
+++

OxidHome is an open home-automation platform built around two ideas:

- **A Rust core** — for memory safety, predictable performance, and a runtime that's small enough to live on the same hardware as your devices.
- **WebAssembly plugins** — so integrations can be written in any language, distributed as portable binaries, and run inside a sandbox that can't reach beyond what the core grants it.

The goal is a hub that's safe to expose to the rest of your home network, fast enough to react in real time, and flexible enough to support the long tail of devices and protocols that make smart-home setups interesting.

## Why Rust + WebAssembly

Smart-home hubs sit in a privileged spot on a home network — they talk to lights, locks, cameras, sensors, and increasingly anything with a radio. That makes two properties non-negotiable: **security** and **reliability**. A crash or a memory corruption bug isn't just an inconvenience; it's a foothold.

Rust gives the core memory safety without a garbage collector, so the runtime stays lean and predictable. WebAssembly gives plugins the same safety guarantees at the boundary: an integration written by anyone, in any language, runs in a capability-scoped sandbox and can only do what the core explicitly permits.

The tradeoff most platforms make — *easy to extend* vs. *safe to extend* — doesn't have to be a tradeoff.
