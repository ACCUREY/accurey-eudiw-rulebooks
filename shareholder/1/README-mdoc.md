# ACC-SHAREHOLDER-1 — mdoc profile (addendum to the SD-JWT VC rulebook)

DocType / namespace: `com.accurey.shareholder.1` (declared to France Identité Partenaires on 20/09/2026).
Same semantics as the SD-JWT VC type `https://vct.accurey.com/shareholder/1`; the nested `company` object is flattened into
`company_name`, `company_id`, `company_id_scheme`, `company_jurisdiction`. `register_as_of` is a full-date in mdoc (date-time in SD-JWT).

Element list, types, mandatory flags, presentation profiles (minimal / band / full), DCQL example and OID4VCI configuration:
see `mdoc.json`.

Trust: MSO signed by an Accurey Document Signer (EKU 1.0.18013.5.1.2) chained to `CN=Accurey IACA, O=ACCUREY, C=LU`,
published on the EUDIW Unfold trusted list. Validity 48 h, re-issued from the register.

Published at `https://vct.accurey.com/shareholder/1/mdoc.json` (application/json, CORS *). Type metadata at `https://vct.accurey.com/shareholder/1`.
