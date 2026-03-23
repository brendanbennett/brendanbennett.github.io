---
title: "Notes on Reproducible Research"
date: 2026-02-10
description: "Some hard-won lessons on making computational research actually reproducible."
---

Reproducibility is one of those things everyone agrees is important and almost nobody does well. I include myself in that criticism. But after a year of trying to re-run my own experiments from six months prior, I've started to develop some habits that help.

These are rough notes, not a manifesto.

## Pin everything

Every dependency. Every version. Every random seed. If your results depend on the phase of the moon, record the phase of the moon. I'm only half joking.

In practice this means:
- A `requirements.txt` or `environment.yml` with exact versions
- Saving the full config for every experiment run
- Using `git` tags to mark the code state for any result you might cite

## Containers are worth the overhead

I resisted Docker for a long time because it felt like overkill for "just some Python scripts." It's not overkill. The two hours you spend writing a Dockerfile will save you twenty hours of debugging CUDA version mismatches on a cluster.

## Write the README before you need it

Future-you is a stranger. Be kind to that stranger. Document how to run things *now*, while the setup is fresh in your mind.

## Automate the pipeline

If getting from raw data to final figure requires more than one manual step, you will eventually get those steps wrong. A Makefile, a shell script, a Snakemake pipeline — anything is better than "oh, you have to run this notebook first, then that one, but skip cell 7."

---

None of this is novel. But sometimes the obvious things are worth writing down, if only so I can point myself back here the next time I'm tempted to skip a step.
