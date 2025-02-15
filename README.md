# `go-libp2p` examples and tutorials

[![](https://img.shields.io/badge/made%20by-Protocol%20Labs-blue.svg?style=flat-square)](https://protocol.ai)
[![](https://img.shields.io/badge/project-libp2p-yellow.svg?style=flat-square)](https://libp2p.io/)
[![](https://img.shields.io/badge/freenode-%23libp2p-yellow.svg?style=flat-square)](http://webchat.freenode.net/?channels=%23libp2p)
[![Discourse posts](https://img.shields.io/discourse/https/discuss.libp2p.io/posts.svg)](https://discuss.libp2p.io)

In this folder, you can find a variety of examples to help you get started in using go-libp2p. Every example as a specific purpose and some of each incorporate a full tutorial that you can follow through, helping you expand your knowledge about libp2p and p2p networks in general.

在此文件夹中，您可以找到各种示例来帮助您开始使用go-libp2p。 每个示例作为特定目的，其中一些包含您可以遵循的完整教程，帮助您扩展您对libp2p和p2p网络的了解。

Let us know if you find any issue or if you want to contribute and add a new tutorial, feel welcome to submit a pr, thank you!

## Examples and Tutorials

- [The libp2p 'host'](./libp2p-host)
- [Building an http proxy with libp2p](./http-proxy)
- [An echo host](./echo)
- [Multicodecs with protobufs](./multipro)
- [P2P chat application](./chat)
- [P2P chat application w/ rendezvous peer discovery](./chat-with-rendezvous)
- [P2P chat application with peer discovery using mdns](./chat-with-mdns)

## Troubleshooting

When building the examples ensure you have a clean `$GOPATH`. If you have checked out and built other `libp2p` repos then you may get errors similar to the one below when building the examples. Note that the use of the `gx` package manager **is not required** to run the examples or to use `libp2p`.
```
$:~/go/src/github.com/libp2p/go-libp2p-examples/libp2p-host$ go build host.go 
# command-line-arguments
./host.go:36:18: cannot use priv (type "github.com/libp2p/go-libp2p-crypto".PrivKey) as type "gx/ipfs/QmNiJiXwWE3kRhZrC5ej3kSjWHm337pYfhjLGSCDNKJP2s/go-libp2p-crypto".PrivKey in argument to libp2p.Identity:
        "github.com/libp2p/go-libp2p-crypto".PrivKey does not implement "gx/ipfs/QmNiJiXwWE3kRhZrC5ej3kSjWHm337pYfhjLGSCDNKJP2s/go-libp2p-crypto".PrivKey (wrong type for Equals method)
                have Equals("github.com/libp2p/go-libp2p-crypto".Key) bool
                want Equals("gx/ipfs/QmNiJiXwWE3kRhZrC5ej3kSjWHm337pYfhjLGSCDNKJP2s/go-libp2p-crypto".Key) bool
```

To obtain a clean `$GOPATH` execute the following:
```
> mkdir /tmp/libp2p-examples
> export GOPATH=/tmp/libp2p/examples
```

---

The last gx published version of this module was: 
