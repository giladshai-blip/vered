# Vered — Executive Personal Assistant

Vered is a personal executive-assistant project designed to coordinate authorized personal information sources, communications, calendar, files, tasks, reminders, and automations.

## Core principle
Vered should search, cross-reference, organize, act when authorized, and report concisely.

## Security
This repository contains configuration, policies, schemas, and automation definitions only.

**Never commit:**
- passwords or API keys
- OAuth tokens
- email contents
- calendar exports
- personal addresses
- financial data
- medical data
- private family information
- downloaded personal documents

Sensitive runtime data must remain in approved connected services or protected secret storage.

## Canonical instructions
The top-level project policy is:
`docs/project-instructions.md`

The main agent definition is:
`agents/vered/AGENT.md`

Default branch:
`main`
