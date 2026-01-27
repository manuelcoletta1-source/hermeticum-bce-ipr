# Livelli IPR (spiegazione semplice)

I livelli misurano la **qualità verificabile dell’evidenza**, non “chi sei”.

## BASE
- record minimo
- digest SHA-512

## VERIFIED
- BASE
- receipt firmata (ED25519) verificabile offline

## STRONG
- VERIFIED
- Evidence Pack completo (`PACK_MANIFEST.json`)
- opzionali anchor esterni (BTC/ETH/IPFS) solo come ridondanza
