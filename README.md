# Distributed Hosting & Benchmarking System

A distributed platform to benchmark and host high-frequency trading infrastructure submitted by contestants. Built in Go, Rust, and TypeScript.

## Architecture Overview

*Architecture diagram coming after Day 19.*

## Stack

| Layer | Technology |
|---|---|
| Sandboxing | Firecracker MicroVM + Intel RDT |
| Load Generation | Go bot fleet + Rust FIX engine (SIMD) |
| Telemetry | eBPF/XDP → Redpanda → QuestDB + ClickHouse |
| Leaderboard | Redis Pub/Sub → WebSocket → Next.js |
| IaC | Terraform + Helm + Cilium |


## Quick Start

```bash
docker-compose up
```

*Full setup guide coming after Day 19.*
