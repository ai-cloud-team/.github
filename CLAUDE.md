# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Что это

`.github` — служебный репозиторий организации **ai-cloud-team**: `profile/README.md` (страница организации), общие issue/PR-шаблоны, reusable GitHub Actions workflows для репо `platform`, `tenants`, `docs`.

## Правила

- `profile/README.md` — позиционирование (D37 в `platform/docs/SYNTHESIS.md`): управляемая AI-команда разработки на разработчика, публичная схема `profile/architecture-{light,dark}.png` (генерируется из `research-local/diagrams/ai-cloud-team-public.architecture.json`). Без внутренних деталей: VK, ASM-пути, NetworkPolicy, имена namespace.
- Reusable workflows (`.github/workflows/*.yml` с `on: workflow_call`): `helm-lint`, `kubeconform`, `python-tests`, `values-schema-check`. Пинить actions по commit SHA (Renovate `helpers:pinGitHubActionDigests`).
- Шаблоны issue — на английском, для публичных `docs`; внутренние шаблоны инцидентов живут в `platform/incidents/`.
