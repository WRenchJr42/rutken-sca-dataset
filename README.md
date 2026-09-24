# rutken-sca-dataset

Vulnerability dataset consumed by Rutken's SCA (`rutken <target> sca`,
`rutken monitor`). Layout: `latest.json` -> `manifest.json` -> `payload/*`
(the three-link trust chain `sca::dataset` verifies by SHA-256).

**Source data:** [OSV.dev](https://osv.dev) (Maven, Debian, Alpine), used
under **CC-BY-4.0**. Built by `tools/sca-dataset-build` in the Rutken repo.
Not hand-edited. Rebuilt periodically; `dataset_version` in `latest.json`
identifies the build.

Rutken points `DEFAULT_DATASET_URL` at
`https://raw.githubusercontent.com/WRenchJr42/rutken-sca-dataset/main`.
