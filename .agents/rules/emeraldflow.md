---
trigger: always_on
---

# EmeraldFlow Project Rules

You are assisting me in building EmeraldFlow, a DevOps portfolio project.

## My Learning Preference

- I am learning DevOps through hands-on project-based learning.
- Do not assume I already understand a technology just because it appears in the project.
- When introducing a new concept, explain it briefly and simply before using it.
- Prefer practical explanations with small examples.
- Do not overwhelm me with unnecessary theory.
- Help me understand what we are doing, not just generate code.

## How You Should Make Changes

- Before changing files, inspect the existing project structure and relevant files.
- Do not modify unrelated files.
- Keep implementations simple and minimal.
- Do not over-engineer.
- Do not introduce new technologies, dependencies, services, or architectural patterns unless they are actually needed.
- Follow the existing project architecture instead of redesigning it.
- If a major architectural decision is required, explain it before making the change.

## Project Architecture

The project uses:

- Python for the application
- Docker for containerization
- GitHub Actions for CI/CD
- Amazon ECR for container images
- Helm for Kubernetes packaging/configuration
- Argo CD for GitOps deployment
- Kubernetes / Amazon EKS for deployment
- Terraform for infrastructure

Repositories:

- emeraldflow-app = application source code
- emeraldflow-helm = Helm charts and Argo CD configuration
- emeraldflow-infra = Terraform infrastructure

Keep these responsibilities separated.

## Naming

The project name is EmeraldFlow.

Use EmeraldFlow naming consistently.

Do not use "vprofile" for new project names, repository names, Helm chart names, Docker image names, or resource names unless it is necessary to reference the original course material.

## Course Adaptation

This project is based on a DevOps course project that originally uses VProfile.

The goal is to preserve the DevOps architecture and learning objectives while adapting the application and naming to EmeraldFlow.

Do not blindly copy the original project.
Do not redesign the entire project either.

Adapt only what is necessary.

## AI Assistance

When generating code or configuration:

1. First inspect the existing files.
2. Determine what needs to change.
3. Make the smallest reasonable change.
4. Explain what changed and why.
5. Validate the result when possible.

If you find an existing implementation that can be reused, prefer modifying it over creating a duplicate.

## Commands

Before running commands that can modify or destroy infrastructure, explain what the command does.

Never automatically run:

- terraform apply
- terraform destroy
- kubectl delete
- git push
- git reset --hard
- destructive file deletion

unless I explicitly ask you to do so.

## Secrets

Never hardcode real credentials, passwords, API keys, AWS credentials, tokens, or private keys.

Use placeholders or appropriate secret mechanisms.

## Communication

Keep explanations concise and practical.

When I ask "what is X?", explain the concept first instead of immediately changing files.

When I ask you to implement something, implement it and briefly explain the important parts afterward.

If something is wrong with my approach, tell me directly and explain why.

Do not make assumptions about requirements that could significantly change the architecture.

If you are unsure, ask me before making a major change.