# Platform Health Check Tool

## Purpose
This repository contains a small Python-based operational tool used to verify the health of a
production-style hosting platform built on AWS.

The tool is designed to complement an infrastructure project by providing
basic service verification from an operator’s perspective.

## What This Tool Does
- Retrieves the ALB endpoint from Terraform output
- Sends HTTP requests to the service
- Determines whether the platform is healthy
- Exits with appropriate status codes for automation

## Why This Exists
In real platform and infrastructure roles, engineers do not only provision systems.
They are also responsible for verifying availability and responding to failures.

This tool demonstrates basic operational automation and health-check logic.

## How to Run
```bash
pip install -r requirements.txt
python3 scripts/check_service.py
