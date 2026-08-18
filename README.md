# Eval Dataset Builder

> [!IMPORTANT]
> Canonical development has been consolidated into [`vigilanty0x/promptops`](https://github.com/vigilanty0x/promptops), under [`packages/eval-dataset-builder`](https://github.com/vigilanty0x/promptops/tree/main/packages/eval-dataset-builder). This repository remains available to preserve its source history and compatibility reference. The imported `0.1.0` package keeps the `eval-dataset-builder` distribution and CLI names. This notice does not claim a package-index transfer or publication.

Canonical synthetic evaluation datasets with deterministic splits.

Offline Python 3.11+ MVP with zero runtime dependencies, deterministic JSON evidence, bounded inputs, a CLI, synthetic tests, and fail-visible errors.

## Usage

```bash
python -m eval_dataset_builder.cli input.json
python -m unittest discover -s tests -v
python scripts/check.py
```

Input is a JSON object matching the public `run(data)` API in `eval_dataset_builder.core`. With no path, the CLI reads stdin.

Apache License 2.0.

