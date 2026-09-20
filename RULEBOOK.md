# ACC-SHAREHOLDER-1 — Shareholder Status Attestation
## Accurey Verifiable Equity · Rulebook v1.0

**Publisher:** Accurey Partners SCSp, Luxembourg (B289636)
**Legal category:** non-qualified Electronic Attestation of Attributes (EAA), eIDAS 2
**VCT:** `https://vct.accurey.com/shareholder/1`
**Schema:** `https://vct.accurey.com/shareholder/1/schema.json`
**mdoc DocType:** `com.accurey.shareholder.1` — profile: `https://vct.accurey.com/shareholder/1/mdoc.json`

`ACC-SHAREHOLDER-1` attests that a natural person holds a shareholding in a given
company — according to the share register maintained on the Accurey platform, as of
an explicit reference date — **without revealing the size of the holding**.

## Formats

| Format | Identifier | Notes |
|---|---|---|
| SD-JWT VC (`dc+sd-jwt`) | vct `https://vct.accurey.com/shareholder/1` | nested `company` object, selective disclosure per claim |
| ISO mdoc (`mso_mdoc`) | DocType / namespace `com.accurey.shareholder.1` | flattened elements (`company_name`, `company_id`, `company_id_scheme`, `company_jurisdiction`, …), `register_as_of` as full-date |

Both carry the same semantics and are issued from the same register. Element mapping, presentation profiles
(minimal / band / full) and a DCQL example are in [`shareholder/1/mdoc.json`](shareholder/1/mdoc.json).

**Trust:** MSO / JWS signed by an Accurey Document Signer (EKU 1.0.18013.5.1.2) chained to `CN=Accurey IACA, O=ACCUREY, C=LU`.
Issuer (test): `https://api.playground.france-identite.gouv.fr/accurey/issue-demo`. Validity 48 h, re-issued on demand.

See the full normative spec, claims table, validity policy and verification
profiles in the repository. First brick of the Accurey Verifiable Equity family.

Not a state-certified solution nor a qualified trust service. © 2026 Accurey.
