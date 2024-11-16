# gareth-ebpf

## Introduction

* Quite simply, an eBPF playground utilising Go.

## Getting Started

```bash
# Mac Only Steps
limactl start --name=ubuntu resources/vm/ubuntu-lima.yaml
limactl shell ubuntu

# Example invocation
cd cmd/packet_counter
go build
go generate

sudo ./packet_counter
2024/11/16 20:42:10 Counting incoming packets on eth0..
2024/11/16 20:42:11 Received 1 packets
2024/11/16 20:42:12 Received 2 packets
2024/11/16 20:42:13 Received signal, exiting..
```