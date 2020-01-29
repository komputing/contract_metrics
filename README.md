# What is it?

Gathers metrics over a set of contracts (e.g. downloaded via [etherscan-contracts-downloader](https://github.com/komputing/etherscan_contract_downloader))

# How to use it?

Start e.g. via `./gradlew run`

then you find a json like this:

```json
[
  {
    "count": 6331,
    "name": "solidity files"
  },
  {
    "count": 3879,
    "name": "contract with a single solidity file"
  },
  {
    "count": 697,
    "name": "all expressions"
  },
  {
    "count": 284,
    "name": "unique expressions"
  },
  {
    "count": 83,
    "name": "non trivial expressions"
  },
  {
    "count": 13941,
    "name": "all notices"
  },
  {
    "count": 3378,
    "name": "unique notices"
  },
  {
    "count": 6,
    "indicator": "+",
    "name": "addition"
  },
  {
    "count": 0,
    "indicator": "-",
    "name": "subtraction"
  },
  {
    "count": 17,
    "indicator": "?",
    "name": "ternary operator"
  },
  {
    "count": 57,
    "indicator": "(",
    "name": "bracket"
  },
  {
    "count": 3,
    "indicator": "*",
    "name": "multiplication"
  },
  {
    "count": 2,
    "indicator": "/",
    "name": "division"
  },
  {
    "count": 17,
    "indicator": "tokenAmount",
    "name": "tokenAmount"
  },
  {
    "count": 5,
    "indicator": "formatDate",
    "name": "format Date"
  },
  {
    "count": 0,
    "indicator": "formatSince",
    "name": "format since"
  },
  {
    "count": 0,
    "indicator": "ensLookup",
    "name": "ENS lookup"
  },
  {
    "count": 0,
    "indicator": "ensReverseLookup",
    "name": "reverseENS lookup"
  },
  {
    "count": 9,
    "indicator": "formatPct",
    "name": "Percentage formatting"
  }
]⏎ 
```

in `out/metrics/indicator_metrics.json`

You can also find a `out/metrics/non_trivial_expressions.lst` which contains all the expressions used in the NatSpecs that are not just a simple variable.

# License

License MIT
