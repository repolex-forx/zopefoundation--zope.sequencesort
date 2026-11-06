# Repolex Knowledge Graph of zopefoundation/zope.sequencesort

RDF knowledge graph data for [zopefoundation/zope.sequencesort](https://github.com/zopefoundation/zope.sequencesort), parsed by [repolex](https://repolex.ai).

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
rlex download zopefoundation/zope.sequencesort
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 7c6ae9042bef8b6fd5959d6a3946d3246d2ce4a6
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 7c6ae9042bef8b6fd5959d6a3946d3246d2ce4a6
│           └── chunk-001.nq.gz
├── blob
│   ├── 034043e1628b277e8c3805e50acd2ac1e6e85255.nq.gz
│   ├── 0ab12fe1e0c8eb6cb0d68fce1b14a2209cdb0def.nq.gz
│   ├── 0dc2f9479404ef8afbe465b5c5d6a0aa23922c08.nq.gz
│   ├── 1cf8f587075561af7691ac48f618eec8d05a8d85.nq.gz
│   ├── 1f321f52abb7db6f79c285bab56e2852dc575699.nq.gz
│   ├── 2806c164989aa9137a6c1860716ae9abccef75ad.nq.gz
│   ├── 28264e387e69b9e3cdbd412b91f93d0105945ad4.nq.gz
│   ├── 4e836f7cc212cadfb31aeaa623a7d0a62718795f.nq.gz
│   ├── 690a3667aa0fd69f4bd7752674b3f641fa22f9f7.nq.gz
│   ├── 717bb607f8a664ec726e9216cbe5c07025598268.nq.gz
│   ├── 79859e06010bf4967c5b4b044afea6ef39742938.nq.gz
│   ├── 9107ff75373f8e46d429fb11eacbcb92601253cd.nq.gz
│   ├── 9ca7c2f25c618faf4d82bc9cd93bb8f4627ac2ca.nq.gz
│   ├── a7054a3ce49be0483ede2ab203f62538f1db053d.nq.gz
│   ├── a8b9c1476bc2bca0b2f0a190e637e349feaf7bb6.nq.gz
│   ├── bf6e2790de85f36381db49fac2c56396955eaabe.nq.gz
│   ├── c15f59fa1960d34bba97b41230b46809d167221c.nq.gz
│   ├── c5508b9f083362a81185d598327e7801d837cb18.nq.gz
│   ├── c6bc734c94a1c6975bb32cb6bc76f040aa0368ef.nq.gz
│   ├── cc8566e64e031a52c36db85938e6666b186ab658.nq.gz
│   ├── ccdedc28073a0ba8303c52c91284a4e7e70bb471.nq.gz
│   ├── d42adf146765ee256320aa6df4dfbd62cc6f9736.nq.gz
│   ├── da7dda921b8d9390a6323e1b66b6d361e9c3ed32.nq.gz
│   ├── e0c1ff882f585335b8deab9e309e7929b86728f2.nq.gz
│   ├── e1f9ad7b3b48377bfbfaa1b380c384ddea24060f.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e741bd749b161a25b03d4139fb82a6770d0d28eb.nq.gz
│   ├── f0ed9d001e553f388470f3a0b5eca7e9269311c7.nq.gz
│   └── f75c2273495b5681b88b737e9e33daadbbf61e2a.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 7c6ae9042bef8b6fd5959d6a3946d3246d2ce4a6.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 37 files
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

[zopefoundation/zope.sequencesort](https://github.com/zopefoundation/zope.sequencesort)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
