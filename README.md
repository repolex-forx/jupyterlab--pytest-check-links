# Repolex Knowledge Graph of jupyterlab/pytest-check-links

RDF knowledge graph data for [jupyterlab/pytest-check-links](https://github.com/jupyterlab/pytest-check-links), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download jupyterlab/pytest-check-links
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 92c89c079d595f8319403fa7d2d1a4df6cf71ad5
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 92c89c079d595f8319403fa7d2d1a4df6cf71ad5
│           └── chunk-001.nq.gz
├── blob
│   ├── 08651d7c885cdb043d9246974eb211f850de7b48.nq.gz
│   ├── 1fe3c535c17942765a0a47c57a961384cc8a862a.nq.gz
│   ├── 251b0d32129cce3e26dc54d6158a44798b12673c.nq.gz
│   ├── 396330bb9729d2ec595617aef79fb28600d86bd7.nq.gz
│   ├── 3994d9e8ca7c59d82e9bcc79b049cd67ec4e8f5b.nq.gz
│   ├── 3a8d6d5cfb424e39a29c3c60469dd7937e057d3e.nq.gz
│   ├── 439de310d5efbec87a1a5f53973158b245ea7f02.nq.gz
│   ├── 4acb538dab10ef54b509296700664f7640b06069.nq.gz
│   ├── 4c69bb5a3e1ae9a57de70a7c5529e1a1b9d506f1.nq.gz
│   ├── 5295e776b63d7adfab3ddad99962cc6f81968909.nq.gz
│   ├── 5455e2711acf1da6a1b75e913dec3bbb0690ebba.nq.gz
│   ├── 60af4c5f16741c7c2fe17cdd9718ae5f6d56d8a4.nq.gz
│   ├── 7076dea0d483cd3fb59ffbe40090c0df0be1ef9d.nq.gz
│   ├── 725feab5ce652dc39f3f2c77b9fd3c90bf049c65.nq.gz
│   ├── 836c027bc503e2670a5a8d14f50d2f35856ce325.nq.gz
│   ├── 8e905e3a8d31cb8a71e51ed50593ac2e5b9f2231.nq.gz
│   ├── 9a86f70b1ea6dc4d1da6c3baf715f820445f974c.nq.gz
│   ├── a71376f845a362fd99f8808209c12bdfaa2e42fc.nq.gz
│   ├── a7cfe2117274423455f5c107d459016d64515828.nq.gz
│   ├── b1c90e96db68e691e0f1fd0a027d5c200ff9572e.nq.gz
│   ├── bab32f0fb57fdda0b7a0372f4a6be5a38ccd4bda.nq.gz
│   ├── baff17d70bcaa0ded8380f88267ec6348c10ab74.nq.gz
│   ├── cd5a50dd77cd1f0c3516c8e36361666ea7b54e3d.nq.gz
│   ├── e28e0ec34bc352922083b66ee32d1afb02b7f9d5.nq.gz
│   ├── e44a857c0a7015595aa12d91e139596251c976ab.nq.gz
│   ├── e54de7fd01deaf0ef70a87c0238d8591a1562590.nq.gz
│   ├── e5b1ec16efbf6dcecc44de8b1e37a48248d1cf76.nq.gz
│   ├── e5fbd24ea79b7a4f15507ed4260920957c17cc85.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f00b7cbfffeec0340e2334691afce83b65dc220c.nq.gz
│   ├── f1b9d5cddb1a484b405417d1169dee299b42915d.nq.gz
│   └── fcdd3e88b66ec9b10362685146ef2a36088e54f3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 92c89c079d595f8319403fa7d2d1a4df6cf71ad5.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 40 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[jupyterlab/pytest-check-links](https://github.com/jupyterlab/pytest-check-links)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
