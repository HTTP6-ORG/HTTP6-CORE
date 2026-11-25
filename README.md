# HTTP6 Core

This repository is a placeholder for future releases of the HTTP6 Core service. The current runnable examples are available on HTTP6.org.

HTTP6 is a proposed protocol that lets a service check whether a person authorized the specific action an AI agent is asking it to take. When one agent delegates work to another, a signed grant links the new worker to the original approval and defines what it may do. The worker signs its own request. Before acting, the receiving service checks the signature, the chain of grants, and its current policy. It records the outcome so a repeated delivery can be recognized and a lost reply can be recovered.

## Try the W1 examples

W1 carries signed requests over HTTPS. In one example, a scientist authorizes ten compute credits for two workers. Each requests six. The provider checks their shared allowance, records one six-credit charge, and leaves four credits available. [Run the W1 examples on HTTP6.org](https://www.http6.org/developers/w1-example/)

## Licensing

HTTP6 is open source under the MIT License, including for commercial use. Teams can sign payloads, send signatures in HTTP headers, implement their own one-time proofs, and check requests against policy and a ledger. [MIT License](LICENSE)

Only the ENI6MA / Pass+ circuit integration requires a separate ENI6MA license. This applies when an application generates or uses a one-time proof produced by that circuit, whether it uses the supplied Pass+ adapter or its own connector. [ENI6MA / Pass+ licensing terms](https://www.http6.org/participate/licensing/)
