# EOSIO Docker Lab

Legacy Docker-based lab environment for installing EOSIO 1.8.1 on Ubuntu 18.04.

This repository was created as supporting material for a university blockchain course. Its purpose was to give students a reproducible environment for exploring blockchain node software, smart-contract infrastructure, command-line tooling, and Docker-based development workflows.

## Educational Context

At the time this lab was created, EOSIO was a relevant blockchain platform for teaching several technical concepts:

- delegated proof-of-stake architecture
- account and permission models
- WebAssembly-based smart contracts
- blockchain node tooling
- containerized developer environments
- trade-offs between performance, decentralization, usability, and governance

This repository should be understood as an academic teaching artifact, not as an endorsement of EOS as an investment, production platform, or current best-practice blockchain stack.

## What This Dockerfile Does

The Dockerfile:

- starts from `ubuntu:18.04`
- installs `wget`
- downloads the EOSIO 1.8.1 Ubuntu package
- installs the EOSIO package inside the container

## Repository Status

This project is preserved for historical and educational reference.

EOSIO 1.8.1 and Ubuntu 18.04 are legacy dependencies. This image is not maintained for production use and should not be used to operate real infrastructure, manage funds, or deploy production smart contracts.

## Intended Use

Use this repository to study:

- how blockchain tooling was packaged and installed
- how Docker can standardize classroom environments
- how blockchain platforms expose node and developer tooling
- how older blockchain architectures can be compared with Bitcoin, Ethereum, and newer smart-contract platforms

## Example Build
docker build -t eosio-docker-lab .

## Example Run
docker run --rm -it eosio-docker-lab bash

Inside the container, verify the EOSIO tooling according to the commands available in the installed package.

## Security and Maintenance Notes
Do not expose this container to the public internet.
Do not use real private keys, wallet files, credentials, or production data.
Do not use this repository as a template for modern production infrastructure.
Treat this as a classroom lab for historical blockchain architecture.
## Related Course Material

This lab was part of a broader blockchain course repository:

lfgramajo/-UFM-Blockchain-Blockchain-3.0
