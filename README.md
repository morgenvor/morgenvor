# Dmitriy Kurganov

**Junior DevOps Engineer** — CI/CD, containers, Kubernetes, observability, infrastructure as code.

I build delivery pipelines end to end: from a `git push` to a verified rollout on a managed
cluster, with immutable artifacts and checks that fail the build instead of the service. I also
build monitoring that proves it works: SLOs, alerts whose delivery is verified, and incident
drills that leave evidence. Based in Ryazan, Russia (UTC+3). Open to office, remote, and relocation.

![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-F46800?style=flat-square&logo=grafana&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

## Featured projects

### [k8s-observability-lab](https://github.com/morgenvor/k8s-observability-lab)

Operating a Kubernetes service on evidence. SLOs are measured from the client's side — 99 %
availability and 95 % of requests under 300 ms over a three-day window — and the alerts on top of
them are multi-window burn-rate rules rather than raw thresholds. A severity-based Alertmanager
route sends `page` mail that links the runbook, the dashboard and the log window of the incident,
while everything else goes to a journal sink that records delivery. Four fault-injection drills
(connection resets, added latency, a broken readiness probe, an OOM kill) write a machine-readable
timeline, and an alert that fires but never arrives fails the drill.

Offline gates — `promtool` rule tests, `kubeconform` rendering, e-mail template and secret scans —
run in CI, and
[what is proven and what is not](https://github.com/morgenvor/k8s-observability-lab/blob/main/docs/verification.md)
is recorded with dates.

### [YandexCloud-CI-CD](https://github.com/morgenvor/YandexCloud-CI-CD)

A Java 17 / Spring Boot service delivered by a webhook-triggered Jenkins pipeline: Gradle build and
tests, Docker image pushed to Yandex Container Registry, Helmfile deployment to Managed Kubernetes,
rollout checks, and an HTTP smoke test.

What it proves: releases are pinned by registry digest instead of a mutable tag, Jenkins works
through a service account with namespace-scoped RBAC only, and every deploy is gated by rollout and
smoke checks. The cloud environment is decommissioned, so the repository ships a Docker Compose
stack that reproduces the same application and database locally.

## Open source

- [ansible-yandex-cloud-inventory](https://github.com/morgenvor/ansible-yandex-cloud-inventory) —
  Ansible dynamic inventory plugin for Yandex Cloud: a fork of
  [mzatolokin/ansible-yandex-cloud-inventory](https://github.com/mzatolokin/ansible-yandex-cloud-inventory)
  with fixes (label contract, pagination, packaging), published to PyPI as
  `ansible-yandex-cloud-inventory-fixed`. The upstream code is not claimed as my own work.

## Currently learning

- Terraform and Ansible: reproducible infrastructure and repeatable host configuration.

## Contact

- Email: lokrost015@gmail.com
- GitHub: [@morgenvor](https://github.com/morgenvor)
- Looking for Junior DevOps / SRE, Linux system administration, or technical support (L2/L3)
  roles — office, remote, or relocation.
