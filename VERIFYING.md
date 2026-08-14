# Verifying this repository

All sealed artifacts are covered by `SHA256SUMS.txt`.

## Verify (any platform)

    git clone --branch v1.0.2 https://github.com/darksciencedivision-ctrl/adversarial-trajectory-graphs.git
    cd adversarial-trajectory-graphs && sha256sum -c SHA256SUMS.txt

Expected: every entry `OK`. Verification also passes at any commit
from v1.0.2 forward, including HEAD of `main`.

## Known limitation — earlier tags

Tags v1.0.1 predate the `.gitattributes` byte-exact checkout rule.
On machines with `core.autocrlf=true` (the Windows default), cloning
at those tags CRLF-converts the manifest itself, so every path gains a
trailing `\r` and `sha256sum -c` reports "No such file or directory"
for every entry. This is a checkout artifact, not repository
corruption: the committed blobs are intact. To verify a historical
seal:

    git clone -c core.autocrlf=false --branch v1.0.1 https://github.com/darksciencedivision-ctrl/adversarial-trajectory-graphs.git

Sealed content at v1.0.2 matches the historical seals except the
author-attribution correction recorded in the commit history
(including regenerated PDF renders).
