# Poki personal compatibility build

Builds an unsigned iPhone app from the public AGPL-3.0-only Poki source at `ZhehanZhang/poki-remote`, commit `10c4f80be7761c83004e41b885121953032518e8`.

The compatibility patch exposes a configurable RemotePairing service port in Diagnostics, passes it through the Swift/Rust launcher, and preserves 49152 as the default. It does not change VPN, DNS, routing or pairing credential handling. A configurable port fixes only a connection prerequisite; the actual phone must still pass pairing and end-to-end operation tests.

This repository contains public source references, build instructions and a source patch only. It contains no signing certificates, Apple account data, phone pairing records or API credentials. Signing happens locally after inspecting the unsigned artifact. See the upstream repository for its AGPL-3.0-only license and source notices. Modified source is available by applying this patch to the pinned commit.
