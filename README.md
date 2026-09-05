# quant-research

A lightweight research lab for economics, finance, accounting, statistics, and quantitative experiments.

## Purpose

This repository is the **discovery and experimentation layer** around Quant-v2.

- **Quant-v2** owns trustworthy data, ingestion, PIT/as-of semantics, reusable production features, and deployable infrastructure.
- **quant-research** consumes those data, asks questions, tests hypotheses, records failed and successful experiments, and proposes reusable discoveries for promotion back into Quant-v2.

The dependency direction should remain one-way at runtime:

```text
Quant-v2 data / API / database
          |
          v
    quant-research
          |
          v
 hypotheses / experiments / findings
          |
          v
 promotion proposal or data request
          |
          v
       Quant-v2
```

Research may request new data from Quant-v2, but research code must not silently become a production ingestion path.

## Initial scope

The first phase is deliberately small:

1. Build minimum usable foundations in economics, finance, accounting, and statistics.
2. Turn concepts into small empirical experiments as early as possible.
3. Keep research notes, notebooks, results, and reusable research utilities separate.
4. Promote only stable, reusable discoveries into Quant-v2 Feature/Factor layers.

## Research lifecycle

```text
Question
  -> Mechanism
  -> Hypothesis
  -> Data required
  -> Experiment
  -> Result
  -> Limitations
  -> Next question
  -> Promotion candidate / Data request
```

This repository is expected to contain failed hypotheses and incomplete experiments. That is normal; it is a research workspace, not a production data repository.
