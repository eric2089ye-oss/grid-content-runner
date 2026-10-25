# Static publishing runner

A minimal scheduled runner. Build inputs and configuration are held in private Cloudflare KV. Repository secrets supply account, project and credential settings.

Runs are serialized. The private runner validates current source data, preserves the approved route set and checks the deployed output. Scheduled runs can be delayed by GitHub; workflow dispatch is available for recovery.

No site content or source collection implementation is stored in this repository.
