# MCP Bench

Benchmark for evaluating LLM tool-call latency across distributed Kubernetes (k3s) clusters.

## Description
This repository contains a Kubernetes manifest (`bench.yaml`) that deploys:
- a proxy node (Frankfurt),
- a remote tool service (Sakhalin),
- a benchmark runner (Moscow),

to evaluate latency under different communication topologies (1x1, 1xM, Nx1, NxM)
using Google Gemini tool calls.

## Requirements
- k3s / Kubernetes cluster
- Google API key (provided via Kubernetes Secret)
