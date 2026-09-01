# JLS JMdict lookup artifact

This repository publishes the mechanical JMdict-derived word lookup dataset
used by Japanese Language Studies. JLS makes no copyright claim over the
upstream dictionary data.

## Source and licence

- Upstream: JMdict_e, maintained by the Electronic Dictionary Research and
  Development Group (EDRDG)
- Project: https://www.edrdg.org/wiki/index.php/JMdict-EDICT_Dictionary_Project
- Snapshot creation date: 2026-08-31
- Snapshot SHA-256: `5f89bc7db70f2656ba78535d83e4bfe9d56fb5f0fe08290e99ecebc3d1386812`
- Licence: Creative Commons Attribution-ShareAlike 4.0 International

The `data/` directory is byte-identical to the generated artifact in JLS. Its
manifest records per-shard hashes and counts.

## Update procedure

On the first of each month, download the current `JMdict_e.gz`, verify and
record its creation date and SHA-256, regenerate the shards, review the
entry/shard summary, publish the artifact here, then import it after the JLS
change has merged. Entries removed upstream are pruned by `ent_seq`.
