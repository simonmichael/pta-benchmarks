# Generic Performance Benchmarks

This directory contains generic benchmark setup
with generated plain text accounting data.

Benchmark results will report used time, memory and CPU utilization for
basic balance report with commodities.

Generated transaction set contains roughly 400 accounts and 31 commodities.

Test setup supports various test set sizes, ranging from 10 (1e1)
to 1_000_000 (1e6) transactions.

Reasonable starting point would be 10_000 (1e4) transactions.


## Installation

Install the [PTA-Generator](https://github.com/tackler-ng/pta-generator):

````
cargo install --locked pta-generator
````

You also need to have [just](https://just.systems/) installed,
and the PTA tools.

### Installation of PTA Tools

Currently tested tools are beancount, hledger, ledger and tackler.

Installation instructions for these are located here:

* Beancount: [Installing Beancount](https://beancount.github.io/docs/installing_beancount.html)
* HLedger: [Install](https://hledger.org/install.html)
* Ledger: [Download](https://ledger-cli.org/download.html)
* Tackler: [Quickstart](https://tackler.e257.fi/docs/quickstart/)


## Usage

After that the usage is super-simple, just run:

````bash
just help
just gen 1e4
just bench 1e4
just version
````

The set size could be `1e1`, `1e2`, ..., `1e5`, `1e6`.

PTA tools are run in order of probable execution time (fastest first).

If the `time` command in the justfile doesn't work for you, then just use
the the other version of `time` in the script.

