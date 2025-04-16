Some rough benchmarks of plain text accounting apps,
currently Ledger, hledger, Beancount, and Tackler.

- 10k - balance report with 10 thousand transactions and 1 thousand accounts
- 100k - balance report with 100 thousand transactions and 1 thousand accounts
- 500k - balance report with 500 thousand transactions and 1 thousand accounts
- generic - benchmark (time, mem, cpu) of balance report with different journal sizes

Tools that may be useful:

- just       - https://just.systems
- quickbench - https://hackage.haskell.org/package/quickbench
- pta-generator     - https://github.com/tackler-ng/pta-generator
- BSD time or GNU time

- ledger     - https://ledger-cli.org
- hledger    - https://hledger.org
- beancount  - https://beancount.github.io
- tackler 25.04.2+    - https://tackler.e257.fi
