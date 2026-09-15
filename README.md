# accurey-eudiw-rulebooks

Public rulebooks for **Accurey Verifiable Equity** — capital & equity attestations,
served resolvable under `https://vct.accurey.com`.

## What resolves where
| URL | File | Purpose |
|---|---|---|
| `https://vct.accurey.com/shareholder/1` | `.well-known/vct/shareholder/1` | SD-JWT VC **type metadata** (what wallets fetch) |
| `https://vct.accurey.com/shareholder/1/schema.json` | `shareholder/1/schema.json` | JSON Schema of the claims |
| `https://vct.accurey.com/RULEBOOK.md` | `RULEBOOK.md` | human-readable norm |
| `https://vct.accurey.com/` | `index.html` | landing page |

> SD-JWT VC resolution: a VCT `https://host/path` is resolved by wallets at
> `https://host/.well-known/vct/path`. Hence the type metadata lives under
> `.well-known/vct/shareholder/1`.

## Licence
Specification under **CC BY 4.0** (attribution to Accurey required).
"Accurey" is a trademark. Issuance authority is reserved to Accurey and authorised
issuers — see `LICENSE`.

© 2026 Accurey Partners SCSp.
