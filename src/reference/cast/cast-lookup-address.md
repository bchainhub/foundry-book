## probe lookup-address

### NAME

probe-lookup-address - Perform an ENS reverse lookup.

### SYNOPSIS

``probe lookup-address`` [*options*] *who*

### DESCRIPTION

Perform an ENS reverse lookup.

If `--verify` is passed, then a normal lookup is performed after the reverse lookup to verify that the address is correct.

### OPTIONS

#### Lookup Options

`-v`  
`--verify`  
&nbsp;&nbsp;&nbsp;&nbsp;Perform a normal lookup to verify that the address is correct.

#### RPC Options

{{#include ../common/rpc-url-option.md}}

{{#include common-options.md}}

### EXAMPLES

1. Get the ENS name for an address.
    ```sh
    probe lookup-address $ADDRESS
    ```

2. Perform both a reverse and a normal lookup:
    ```sh
    probe lookup-address --verify $ADDRESS
    ```

### SEE ALSO

[probe](./probe.md), [probe resolve-name](./probe-resolve-name.md)
