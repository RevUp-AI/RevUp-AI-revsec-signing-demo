# RevSec signing demo

> [!CAUTION]
> **Test artefact for the RevSec package-integrity check. Do not install, run or depend on it.**
> It contains no working code.

RevSec records a fingerprint of an MCP server's published package and checks it again whenever someone approves the
server. If the published package has changed since the fingerprint was recorded, RevSec refuses the approval unless
the reviewer deliberately overrides it, and it writes the override to the audit trail.

This repository is the "published package" for demonstrating that check. During a demo, release `v1.0.0` is
re-pointed to a different commit after RevSec has recorded its fingerprint. That is what an attacker does when they
take over a release: the version number stays the same while the contents change.

There is nothing here worth using.
