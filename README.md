# DevOps CI/CD Assessment

## Overview
This project demonstrates an automated CI/CD pipeline that prevents broken code from reaching the main branch.

## Tools Used
- GitHub Actions (CI/CD Pipeline)
- Python + Pytest (Application & Tests)
- Git Branches (Feature isolation)

## How It Works
Every time code is pushed, GitHub Actions automatically runs tests. If tests fail, the code is blocked.

## Scenario A - Happy Path
Clean code is pushed → Tests pass → Pipeline shows green

## Scenario B - Breaking Path  
Broken code is pushed → Tests fail → Pipeline blocks it automatically

## Workflow Rules
- All pushes trigger the pipeline
- Tests must pass before merging to main
- Failed pipelines block bad code automatically
