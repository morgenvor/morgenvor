# Dmitriy Kurganov

**Junior DevOps Engineer** — CI/CD, containers, Kubernetes, infrastructure as code.

I build delivery pipelines end to end: from a `git push` to a verified rollout on a managed
cluster, with immutable artifacts and checks that fail the build instead of the service.
Based in Ryazan, Russia (UTC+3). Open to office, remote, and relocation.

![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

## Featured project

### [YandexCloud-CI-CD](https://github.com/morgenvor/YandexCloud-CI-CD)

A Java 17 / Spring Boot service delivered by a webhook-triggered Jenkins pipeline:
Gradle build and tests, Docker image pushed to Yandex Container Registry, Helmfile
deployment to Managed Kubernetes, rollout checks, and an HTTP smoke test.

What it proves: releases are pinned by registry digest instead of a mutable tag, Jenkins
works through a service account with namespace-scoped RBAC only, and every deploy is
gated by rollout and smoke checks.

The cloud environment is decommissioned, so the repository ships a Docker Compose stack
that reproduces the same application and database locally.

## Currently learning

- Prometheus and Grafana: metrics collection, dashboards, and alerting rules for
  Kubernetes workloads.
- Terraform and Ansible: reproducible infrastructure and repeatable host configuration.

## Contact

- Email: lokrost015@gmail.com
- GitHub: [@morgenvor](https://github.com/morgenvor)
- Looking for Junior DevOps / SRE roles — office, remote, or relocation.
