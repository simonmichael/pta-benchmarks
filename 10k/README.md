This benchmark runs a balance report on a journal with
10k transactions, 1k accounts at 10 depths, about 6k costs, and 26 commodities.

Currently, it tests ledger, hledger, and tackler on this file.
It also tests tackler with the file split into 28 per-year files.

The file has also been split into 329 per-month files, but those aren't currently used.

There's also a variant with a simpler journal
(about 400 accounts at 4 depths, no costs, 1 commodity).
