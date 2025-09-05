# Gossamer-Jam Binary Releases

This repository contains the binary releases of Gossamer-Jam.

Gossamer-Jam is a [JAM](https://graypaper.com/) Node implementation in Golang by ChainSafe.

## Testing the Implementation against a Fuzzer

To test the implementation ("target") against the [JAM protocol conformance testing tool](https://github.com/davxy/jam-stuff/blob/main/fuzz-proto/README.md) ("fuzzer"),
run it using the `target` command:

```
Run the implementation as a target for the JAM protocol conformance testing tool ("fuzzer"). For more information: https://github.com/davxy/jam-stuff/blob/main/fuzz-proto.

Usage:
  gossamer-jam target [flags]

Flags:
  -h, --help            help for target
  -s, --socket string   UNIX Domain Socket Address to connect to (default "/tmp/jam_target.sock")
```

In this mode, the fuzzer communicates with the target using a synchronous request-response protocol over a Unix domain socket.
