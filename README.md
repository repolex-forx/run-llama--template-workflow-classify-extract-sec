# Repolex Knowledge Graph of run-llama/template-workflow-classify-extract-sec

RDF knowledge graph data for [run-llama/template-workflow-classify-extract-sec](https://github.com/run-llama/template-workflow-classify-extract-sec), parsed by [repolex](https://repolex.ai).

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
rlex download run-llama/template-workflow-classify-extract-sec
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── bc83c5739dc0c667180609d3d77eb4a73312623e
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── bc83c5739dc0c667180609d3d77eb4a73312623e
│           └── chunk-001.nq.gz
├── blob
│   ├── 06dbd0374c7d138c40ed5b5486a26d1cdbbd6cca.nq.gz
│   ├── 1bd7e75eb30d851dfcb2a0735b070e4b5a9a0c31.nq.gz
│   ├── 1db54c3f1357df8c6f65f2ecb4bd4580bf18b551.nq.gz
│   ├── 25ad5bcbea25ab78a63bd3f3f84a66693ffa7f2f.nq.gz
│   ├── 35fca6eac9cae2583c8c1de898b60f793a1ec092.nq.gz
│   ├── 3cdee003bf488e12d3a4fa4953119126da830f87.nq.gz
│   ├── 453877564ffaa7b88a1f0ee26a55af5ab35e4cd4.nq.gz
│   ├── 45b37fc91442a293c8805c74bf853e259bab8ed1.nq.gz
│   ├── 4da33406e72b559c03d608dd6285862cf3587d83.nq.gz
│   ├── 5e13111b909c292f8edc2f6499d5d8bfba3214f2.nq.gz
│   ├── 6e995ceb36d85275bec36ddfe2b6c2afa65b7572.nq.gz
│   ├── 6fa106702b614ba5fa6b97a24ff2b6c53c7f9f81.nq.gz
│   ├── 74e78e15b0878064ccc49db36a4c2314f1182643.nq.gz
│   ├── 79ae4b5153e737127849ad8828d2d3328bdc19dd.nq.gz
│   ├── 800bc6ad052fd0f8c6b71ae928ab138a3f6e430a.nq.gz
│   ├── 841950ec45e4674f8483b47f8f14d5bbacd459ee.nq.gz
│   ├── 85c9a64cc53f6202cf5a66bcb8da2b80d60a1090.nq.gz
│   ├── 881adaad2217aa75f669d37cfd3cdf46e64c56c4.nq.gz
│   ├── 88acac8845cf45be2f401aa449d0fcf2f5b786c3.nq.gz
│   ├── 8b8fbda3cc377b013fd8b279243614b544b65a49.nq.gz
│   ├── 8f936fb7733e9c32162bb937642cf7d692dba123.nq.gz
│   ├── 97856e842efe3cace2180a4d1171b10594a84831.nq.gz
│   ├── b1f3492860feb8fe54d06551703182c6259ca77e.nq.gz
│   ├── b56bed7e80ac87ea7ce50913ef870f0db71980f1.nq.gz
│   ├── bb158d8cbb9cee365d0948944819541b12675536.nq.gz
│   ├── c01805e89c1684e79130151abc23bb80401583a9.nq.gz
│   ├── c5283441ea6dd41061b5a83f336fd6cdcacb63c2.nq.gz
│   ├── c5da6423128173b14442dc855c06a1d535726117.nq.gz
│   ├── d0b87119df3aa362010f2522cff0b2fc57f21c4a.nq.gz
│   ├── d8e401fe8f32fff3f18b4763baf4bb4fd63725b4.nq.gz
│   ├── da0ca7eb07bf1ddc4f8b92d2fc74fd43a72d91b3.nq.gz
│   ├── e5439b09bd058b9bbf5e3dc61d7f5eae6eb306eb.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f900b7ec6513a252686e4363d6232bd846bb3b59.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── bc83c5739dc0c667180609d3d77eb4a73312623e.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 40 files
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

[run-llama/template-workflow-classify-extract-sec](https://github.com/run-llama/template-workflow-classify-extract-sec)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
