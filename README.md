# Repolex Knowledge Graph of adamchainz/django-permissions-policy

RDF knowledge graph data for [adamchainz/django-permissions-policy](https://github.com/adamchainz/django-permissions-policy), parsed by [repolex](https://repolex.ai).

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
rlex download adamchainz/django-permissions-policy
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 694b936384b4059b3557a24e174a712fd38abb92
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 694b936384b4059b3557a24e174a712fd38abb92
│           └── chunk-001.nq.gz
├── blob
│   ├── 0123942cce152af307381b0489c995befcd7f75d.nq.gz
│   ├── 0a15aff1b5e41b59d5efafccde7fe10f5621ab03.nq.gz
│   ├── 114b5b422474561be69ad3ccd3639ef16c8ff482.nq.gz
│   ├── 114f638c2e00d2a4d77cfdbc0d7c9690c03e9c8a.nq.gz
│   ├── 13b0f8266b055eee6ef5980a95449f9b695b48b2.nq.gz
│   ├── 205ab9ad9df4ab629d1b7b8d8a72b41f44d8824c.nq.gz
│   ├── 22ddbb118475b52ce8ecba56d9ec45009923da58.nq.gz
│   ├── 2544f7f1002885c36b8dcfe85cba31e3f08436cf.nq.gz
│   ├── 2a7f84f54867d02714727f82eef95d3be939d666.nq.gz
│   ├── 3ba13e0cec6cbbfd462e9ebf529dd2093148cd69.nq.gz
│   ├── 40f4ac757715bb1a8c355eda9124141fdda3aeff.nq.gz
│   ├── 438d629c3ce988e3afffa71110b9660853d38549.nq.gz
│   ├── 4b8b7d0085a188a770f2b1c00fc2fe134b43b922.nq.gz
│   ├── 4b8e8ac1e669c39c3ddb99b03b87b19661de9380.nq.gz
│   ├── 4d880ef16f940023e6ffce4108aeebfcf7feaf49.nq.gz
│   ├── 6acd06f64d1a571e242b60613149e30f2644f2b0.nq.gz
│   ├── 76a4b0f03e51caa9d7dbe83c14c59ae961de4c43.nq.gz
│   ├── 9100ba481d47896cc21b4a4e377d34d8a59f685d.nq.gz
│   ├── 93acb639926ccf42e9a2f76f02419eeaf0405c3a.nq.gz
│   ├── a0be1dd2bc71ab51933650eab41cb02d24ba3e58.nq.gz
│   ├── d10f4d1c923e28fd90318825c52bd1f9999747f9.nq.gz
│   ├── dea0450b9829c75c1a4e0bf11c38488d54aaea7d.nq.gz
│   ├── e66ca36ed06589721b6ae1dd05ad04dcca9d32e2.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ebf65491d8e96aa7680a91efb5f17885dcac45f8.nq.gz
│   └── fc800c6d9c6aac568df8a66ad391bfa8bce43a56.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 694b936384b4059b3557a24e174a712fd38abb92.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 34 files
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

[adamchainz/django-permissions-policy](https://github.com/adamchainz/django-permissions-policy)

---
*Parsed on 2026-10-18 by [repolex](https://repolex.ai)*
