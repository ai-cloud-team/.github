# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Что это

`.github` — служебный репозиторий организации **ai-cloud-team**: `profile/README.md` (страница организации), общие issue/PR-шаблоны, reusable GitHub Actions workflows для репо `platform`, `tenants`, `docs`.

## Правила

- `profile/README.md` — одно короткое описание продукта («Personal AI assistants that run in your cloud…»), ссылки на `docs` и статус проекта. Без внутренних деталей.
- Reusable workflows (`.github/workflows/*.yml` с `on: workflow_call`): `helm-lint`, `kubeconform`, `python-tests`, `values-schema-check`. Пинить actions по commit SHA (Renovate `helpers:pinGitHubActionDigests`).
- Шаблоны issue — на английском, для публичных `docs`; внутренние шаблоны инцидентов живут в `platform/incidents/`.
