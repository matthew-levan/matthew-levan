# Matthew LeVan

Systems engineer working on language runtimes, persistence, functional and distributed systems, 
and correctness, mostly in C and sometimes Rust. Core contributor to [Vere](https://github.com/urbit/vere), 
the C runtime for Urbit, since 2022. Previously worked on build systems, applications, and 
data engineering at Tlon, Wexpert Systems, Clearview AI, and Honeywell Aerospace.

## What I've worked on

**Persistence & storage**
- Epoch system for event-log segmentation and migration ([vere#459](https://github.com/urbit/vere/pull/459))
- `book`: replacing LMDB with a purpose-built event log ([vere#936](https://github.com/urbit/vere/pull/936), [design](https://github.com/urbit/UIPs/pull/82))
- File-backed storage for large atoms ([vere#985](https://github.com/urbit/vere/pull/985), [vere#1121](https://github.com/urbit/vere/pull/1121))
- [Seguro](https://github.com/wexpertsystems/seguro): a replicated event-log storage experiment on FoundationDB

**Memory & runtime internals**
- 64-bit runtime and loom migration ([vere#970](https://github.com/urbit/vere/pull/970))
- Persistent Nock caching + refactor of pointer-compression to compile-time + UIP-0103 ([vere#508](https://github.com/urbit/vere/pull/508))
- Windows port work: demand paging and sparse loom ([vere#1081](https://github.com/urbit/vere/pull/1081))
- Process split (Mars/Urth) between the event processor and I/O driver ([vere#811](https://github.com/urbit/vere/pull/811))

**Rust**
- Wrote most of the crypto jets (native accelerations of Hoon standard-library
  functions) for Ares, the Rust Nock interpreter now maintained as
  [Sword](https://github.com/zorp-corp/sword). Original PR history was
  removed when the project changed hands.

**Correctness**
- Fixed UB in LMDB's misaligned loads ([vere#843](https://github.com/urbit/vere/pull/843)) and an out-of-bounds read in `u3r_bytes` ([vere#1091](https://github.com/urbit/vere/pull/1091))

**Build & release**
- Zig build system, cross-platform CI (Linux/macOS/Windows, x86_64/aarch64), [nixpkgs packaging](https://github.com/NixOS/nixpkgs/pull/216731)

## Tools
C · Rust · Zig · Hoon/Nock · LMDB · FoundationDB · libuv · Nix

## Contact
matthew@coeli.network · consulting via Coeli Network LLC
