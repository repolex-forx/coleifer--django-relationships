# Repolex Knowledge Graph of coleifer/django-relationships

RDF knowledge graph data for [coleifer/django-relationships](https://github.com/coleifer/django-relationships), parsed by [repolex](https://repolex.ai).

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
rlex download coleifer/django-relationships
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 3574799fe5c1971d9b910e6d06814ed8ef585f77
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 3574799fe5c1971d9b910e6d06814ed8ef585f77
│           └── chunk-001.nq.gz
├── blob
│   ├── 00f8d97c4ef7345a125d5fab0da61279a50bd45c.nq.gz
│   ├── 019e31eecb39f43631333c407345fbe6cfe62425.nq.gz
│   ├── 051b6d009496e9b96bc3de741e6be0587ff0c059.nq.gz
│   ├── 092e6c0bc9d49048223a65fa10c0e745bf116c65.nq.gz
│   ├── 0dcfd3228670a57d4f20ce47fc9199324c068dc5.nq.gz
│   ├── 16a6a993da3f343af73c6d04220336246e963e04.nq.gz
│   ├── 1a323362be31c5055b2901813379e974351f0ad9.nq.gz
│   ├── 2300c841282485ddc32956d7f9ed315bcc852d52.nq.gz
│   ├── 241d3c8f4b94415560ddd0f7df180eb6d88f8ade.nq.gz
│   ├── 25158fff896e1a25fdf91170213ce8e6d8500d26.nq.gz
│   ├── 264f99bb070dfdb02818ecc4dd418ab2b7b5441b.nq.gz
│   ├── 2920d6657afa3a80c01378ddf55dd13189341832.nq.gz
│   ├── 2b2c672288937cf5e0f839a043c58537c3966747.nq.gz
│   ├── 2e2bdfaa13ebd87a5fc93128733d36f0a7b82b70.nq.gz
│   ├── 30c050690c9b6dee5f83ed95996da74c435e849d.nq.gz
│   ├── 3bfb04ad789de875b3041259aead7836b7010de5.nq.gz
│   ├── 4deff5aab94ec3e23de363dd2de61d919a78005f.nq.gz
│   ├── 515c651da1a386208bdc5664454c64c821875742.nq.gz
│   ├── 5381ba22d8465093e9a3837f638129429547d7f9.nq.gz
│   ├── 766a8a300b736a97f400ece71dfdccf92f06ae5c.nq.gz
│   ├── 7a083b8c90cf053c0187d9b8ed3e4eaeaff226f6.nq.gz
│   ├── 90af01428b245bb9bee7e662c374837a7cdd7b63.nq.gz
│   ├── 93120e66c81f4b26c1d40a4b853394b85131e9ed.nq.gz
│   ├── 985a9c7928ab312518835bdb72d9f712cca8632a.nq.gz
│   ├── 9b5c4cea6ff2fa6a12908c0a37497457e95ea657.nq.gz
│   ├── 9d30792e23de3ebf9fbdb7fac40a46154a2115ad.nq.gz
│   ├── 9df0c8eb553b4b7ec7bf4ff9987a50aacb9926c4.nq.gz
│   ├── 9fecc3d79ee8f7359a5882e19a3d2f4a3a73725d.nq.gz
│   ├── a286480f2ed579aa6dc5554ca506f580118c7428.nq.gz
│   ├── a5894a511dce1425d9ebb77ae935433cd8f2226e.nq.gz
│   ├── acd1cd0deb42cf9204e1bdee7608b0844b4e9828.nq.gz
│   ├── b660afe8baa266c24f8ec6f8a07c832ab828450c.nq.gz
│   ├── b9f7e96353780830d723298750090c746ec8ce94.nq.gz
│   ├── cd4abe5c53803f6921a442fcc0b1d92364a36f85.nq.gz
│   ├── d1d7d175d39e1bb99db7477351e0e9f80f1cbdbc.nq.gz
│   ├── d860b262ea56d00af52af16552c19428deb78751.nq.gz
│   ├── db9785ec85661a09db6d2d45f27b681a2e9b6437.nq.gz
│   ├── dec4e8ab6e16d906500be4c367cc5d82ed745c12.nq.gz
│   ├── e3151434d38a9c4436b23424e447fd280f7a8255.nq.gz
│   ├── e558856497f459006e071d6ce10b821d372e531b.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── ef7a052e18129b299ae2d8c09fe8af85e506dfe6.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 3574799fe5c1971d9b910e6d06814ed8ef585f77.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 50 files
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

[coleifer/django-relationships](https://github.com/coleifer/django-relationships)

---
*Parsed on 2026-10-20 by [repolex](https://repolex.ai)*
