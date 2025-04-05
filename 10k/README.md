There are two sets of benchmarks here.

The first runs a balance report on a journal with
10k transactions, 1k accounts at 10 depths, about 6k costs, and 26 commodities.
It tests ledger, hledger, beancount and tackler on this file.
It also tests tackler with the file split into 28 yearly files.
(The file has also been split into 329 monthly files, but those aren't currently used.)

The second is a variant with a simpler journal,
with about 400 accounts at 4 depths, no costs, and 1 commodity.

Outputs can be saved from the various benchmark commands.
These should be compared to make sure all apps are performing the same task.

At the time of writing, they look good (equivalent) for the simple benchmark,
but not for the more complex one.

Run `just` to see the available recipes.
