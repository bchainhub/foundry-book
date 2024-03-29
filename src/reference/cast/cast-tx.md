## probe tx

### NAME

probe-tx - Get information about a transaction.

### SYNOPSIS

``probe tx`` [*options*] *tx_hash* [*field*]

### DESCRIPTION

Get information about a transaction.

If *field* is specified, then only the given field of the transaction is displayed.

### OPTIONS

#### RPC Options

{{#include ../common/rpc-url-option.md}}

{{#include ../common/display-options.md}}

{{#include common-options.md}}

### EXAMPLES

1. Get information about a transaction:
    ```sh
    probe tx $TX_HASH
    ```

2. Get the sender of a transaction:
    ```sh
    probe tx $TX_HASH from
    ```

### SEE ALSO

[probe](./probe.md), [probe receipt](./probe-receipt.md)
