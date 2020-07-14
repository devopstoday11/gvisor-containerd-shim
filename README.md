> NOTE: This repository is no longer maintained. The gVisor containerd shims are now
> maintained as part of the core [gVisor](http://www.github.com/google/gvisor/tree/master/shim)
> repository.

# gvisor-containerd-shim

[![Build Status](https://travis-ci.org/google/gvisor-containerd-shim.svg?branch=master)](https://travis-ci.org/google/gvisor-containerd-shim)
[![Go Report Card](https://goreportcard.com/badge/github.com/google/gvisor-containerd-shim)](https://goreportcard.com/report/github.com/google/gvisor-containerd-shim)

gvisor-containerd-shim is a containerd shim for [gVisor](https://github.com/google/gvisor/). It implements the containerd v1 shim API. It can be used as a drop-in replacement for [containerd-shim](https://github.com/containerd/containerd/tree/master/cmd/containerd-shim) (though containerd-shim must still be installed). It allows the use of both gVisor (runsc) and normal containers in the same containerd installation by deferring to the runc shim if the desired runtime engine is not runsc.

## Requirements

-   gvisor (runsc) >= 2018-12-07
-   containerd, containerd-shim >= 1.1

## Installation

-   [Untrusted Workload Quick Start (containerd >=1.1)](docs/untrusted-workload-quickstart.md)
-   [Runtime Handler/RuntimeClass Quick Start (containerd >=1.2)](docs/runtime-handler-quickstart.md)
-   [Runtime Handler/RuntimeClass Quick Start (shim v2) (containerd >=1.2)](docs/runtime-handler-shim-v2-quickstart.md)

## Configuration

-   [Configure containerd-shim-runsc-v1 (shim v2) (containerd >= 1.3)](docs/configure-containerd-shim-runsc-v1.md)
-   [Configure gvisor-containerd-shim (shim v1) (containerd &lt;= 1.2)](docs/configure-gvisor-containerd-shim.md)

# Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).
