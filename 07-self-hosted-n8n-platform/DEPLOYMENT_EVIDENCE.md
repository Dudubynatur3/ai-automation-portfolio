# Self-Hosted n8n Deployment Evidence

## Scope

This case study combines evidence from more than one self-hosted n8n environment. The environments are documented separately here so the portfolio does not merge every component into one unsupported production claim.

## Environment A: local Docker n8n instance

A verified local setup used the official n8n Docker image with a persistent Docker volume.

Recovered command pattern:

```powershell
docker run -d `
  --name n8n-assignment `
  -p 5681:5678 `
  -v n8n_assignment_data:/home/node/.n8n `
  docker.n8n.io/n8nio/n8n:latest
```

The container logs confirmed n8n initialized successfully and listened internally on port `5678`, exposed locally through port `5681`.

This environment was used during workflow implementation and testing.

## Environment B: wider messaging / automation stack

A separate older development environment included multiple services supporting WhatsApp / Chatwoot automation work.

Recovered components include:

- n8n
- PostgreSQL
- Redis
- Chatwoot
- `chatwoot_sidekiq`

Recovered service-port context includes:

- n8n on port `5678`
- Chatwoot on port `3000`

The environment contained approximately **21 workflows** in the recovered n8n data set. That number is treated as development-environment evidence, not as a claim that 21 workflows were production deployments.

Named workflow evidence recovered from that environment includes examples such as:

- `WhatsApp Order Processor (Twilio) Final`
- `WF2 — One-Click Lead Ingestion`

Some older workflows used simulated or mocked external integration steps. They are therefore not represented as live production integrations.

## Environment C: production-style hosting pattern

Separate project records also document work with a production-style n8n hosting pattern using:

- Docker / Docker Compose
- PostgreSQL persistence
- Redis
- Traefik reverse proxying
- HTTPS
- custom-domain routing

The public portfolio does not publish an exact Docker Compose file for this environment until the original configuration is recovered and reviewed for secrets and environment-specific values.

## Why the distinction matters

It would be easy to write one oversized claim such as:

> Deployed n8n, PostgreSQL, Redis, Traefik, Chatwoot and 21 production workflows.

The recovered evidence does **not** support that exact statement.

The defensible claim is narrower:

> Self-hosted n8n across Docker-based environments, worked with PostgreSQL/Redis persistence and a wider Chatwoot messaging stack, and used reverse-proxy/HTTPS/custom-domain patterns in production-style hosting work.

## Skills demonstrated

- Docker-based n8n hosting
- persistent n8n data volumes
- container logs and migration monitoring
- PostgreSQL / Redis platform components
- Chatwoot integration environment
- multi-service Docker architecture
- reverse proxy concepts
- HTTPS / custom-domain deployment patterns
- workflow backup and recovery awareness
- clear separation of development, demo, and production evidence
