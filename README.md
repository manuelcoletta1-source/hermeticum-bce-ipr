# IPR — Identity Primary Record (Gateway)

IPR è un **record tecnico minimo** che rende verificabile nel tempo
la continuità operativa di un soggetto tramite evidenze crittografiche.

## Principi
UE_FIRST · GDPR_MIN · HASH_ONLY · FAIL_CLOSED · AUDIT_FIRST

## Output
- `ipr.json` / `ipr.canon.json`
- `receipt.json` (firma ED25519 su digest SHA-512)
- `PACK_MANIFEST.json` (Evidence Pack)
- `anchor-pack.json` (opzionale)

## FAIL-CLOSED (regola)
Se una verifica fallisce (hash/firma/manifest), l’IPR è **non valido**.

## Livelli
- BASE: record + digest
- VERIFIED: BASE + receipt verificabile
- STRONG: VERIFIED + Evidence Pack completo (+ opzionali anchor)

## Non è
- identità civile
- sostituto eIDAS/EUDI
- promessa di valore legale automatico

## Collegamenti
- Gateway UE: https://manuelcoletta1-source.github.io/hermeticum-bce-platform/
- UNEBDO: https://manuelcoletta1-source.github.io/unebdo/
- OPC: https://manuelcoletta1-source.github.io/opc/
- B2B: https://manuelcoletta1-source.github.io/hermeticum-bce-b2b/
- B2G: https://manuelcoletta1-source.github.io/hermeticum-bce-b2g/
