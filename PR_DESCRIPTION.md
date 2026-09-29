## Summary

Closes #171

This change preserves and publishes the number of distinct candidate paths considered for each priced rung.

## What changed

- count distinct Horizon paths before dropping the lower-ranked candidates
- carry the count through route pricing into the published quote model
- expose the value on rung and recommended quote JSON as 
- add a regression test covering the wire output contract

## Why

The previous behavior discarded all but the best path for a rung, which meant the published corridor data lost legitimate path diversity even when Horizon returned several viable routes.

## Verification

- ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/analysis	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/anchor	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/asset	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/checks	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/cmd/hop-analysis	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/cmd/ladder	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/cmd/stellar-co-star-stellar-co-star-stellar-co-star-wayfared	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/dex	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/monitor	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/refrate	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/route	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/runstore	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/sep38	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/server	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/snapshot	(cached)
ok  	github.com/stellar-co-star/stellar-co-star-stellar-co-star-stellar-co-star-wayfare/transport	(cached)
