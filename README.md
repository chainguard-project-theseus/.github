# Project Theseus
 
Chainguard's Project Theseus is an effort to rebuild the core components
of open source and eliminate entire classes of bugs. We're doing it one
component at a time, in the open.
 
## Why
 
The open source software the world runs on was built for a different
threat landscape. Finding bugs has gotten much faster than fixing them:
AI finds bugs around the clock, and every fix still has to be written,
reviewed, released and deployed. Many of those bugs come from the same
few kinds of mistakes.
 
# Project Theseus

Chainguard's Project Theseus is an effort to rebuild the core components
of open source and eliminate entire classes of bugs. We're doing it one
component at a time, in the open.

## Why

The open source software the world runs on was built for a different
threat landscape. Finding bugs has gotten much faster than fixing them:
AI finds bugs around the clock, and every fix still has to be written,
reviewed, released and deployed. Many of those bugs come from the same
few kinds of mistakes.

Project Theseus rewrites core components so that entire classes of
mistakes can't happen in them, starting with memory-safety bugs.

## Guarded Components

Each repository here holds a Guarded Component, a replacement for a core
open source component, built so a whole class of bugs isn't possible in
it. Some are rewrites we build with AI agents and others are existing
rewrites that we adopt and harden. Both are held to the same bar:

- **Tested against the original.** Each one is fuzzed against the
  component it replaces and tested across Chainguard's catalog of more
  than 3,000 production images before it becomes a default.
- **Evidence in the open.** We publish conformance results and
  performance comparisons as they're ready, and formal proofs for the
  most critical pieces.

Drop-in rewrites we build use a `cg-` prefix. Components that are new
designs keep their own names.

## Components

- **[challoc](https://github.com/chainguard-project-theseus/challoc)**: a
  memory allocator written in Rust, built to replace glibc malloc,
  jemalloc, tcmalloc and mimalloc. Status: experimental.

## Get involved

Try a component in a test environment. If something breaks or behaves
differently from the component it replaces, file an issue in
[chainguard-project-theseus/feedback](https://github.com/chainguard-project-theseus/feedback/issues).

We aren't accepting pull requests.

For the full story, read the blog introducing Chainguard Project Theseus and
[Rebuild the planet](https://www.chainguard.dev/unchained/rebuild-the-planet).

## Trademarks

Use of the Chainguard and challoc names, as well as other Chainguard
trademarks, logos, and brand assets, is governed by the
[Chainguard Trademark Use Policy](https://www.chainguard.dev/legal/chainguard-trademark-use-policy).
