
# Unified Operations Console

Unified Operations Console (UOC) is a centralized operations console for managing servers, infrastructure, security, and administration across all entities.

## Overview

UOC brings day-to-day infrastructure operations into one organized control surface. It helps operations teams understand environment state, perform administrative actions, respond to incidents, and maintain consistent governance across multiple entities and services.

The project is built on the Apache CloudStack codebase and is organized as a modular platform with management services, APIs, agents, storage integrations, network services, plugins, system virtual machines, and a web interface.

## Operational Scope

- **Server and compute management**: Provision, monitor, operate, and retire compute resources.
- **Infrastructure management**: Coordinate zones, pods, clusters, hosts, storage, networks, and capacity.
- **Security administration**: Manage identities, access controls, credentials, network boundaries, and policies.
- **Entity administration**: Organize users, accounts, domains, projects, and delegated responsibilities.
- **Network operations**: Manage virtual networks, public addresses, routing, firewalls, load balancing, and VPN services.
- **Storage operations**: Work with primary and secondary storage, templates, snapshots, volumes, and backups.
- **Availability and maintenance**: Support host maintenance, service health, capacity planning, and recovery workflows.
- **Automation and integration**: Expose APIs and extension points for external systems and infrastructure tooling.

## Core Capabilities

- Centralized management of distributed infrastructure
- Multi-entity administration with role-based access control
- Virtual machine, volume, template, snapshot, and ISO lifecycle operations
- Account, user, domain, project, and resource-limit management
- Network, IP address, firewall, NAT, load-balancer, and VPN administration
- Host, cluster, storage-pool, and capacity visibility
- Events, alerts, asynchronous jobs, and operational audit information
- Pluggable hypervisor, storage, network, authentication, and backup integrations
- API-driven automation for console and external operations workflows

## Architecture

The repository contains the major platform layers needed to operate a cloud and infrastructure management system:

- `api/` contains public API definitions and API-facing models.
- `client/` contains client-side and command-line integration components.
- `core/` contains shared domain and platform logic.
- `engine/` contains orchestration, service, storage, schema, and userdata components.
- `framework/` contains jobs, events, security, REST, and configuration support.
- `plugins/` contains pluggable providers and integrations.
- `server/` and `services/` contain management and supporting services.
- `systemvm/` contains system virtual machine components.
- `ui/` contains the web console.
- `test/` contains test and integration resources.

## Typical Workflow

1. Register and organize infrastructure resources.
2. Configure compute, storage, networking, and security policies.
3. Assign users and entities the permissions required for their responsibilities.
4. Provision and operate workloads through the console or API.
5. Monitor events, capacity, jobs, and service health.
6. Apply maintenance, backup, recovery, and lifecycle operations consistently.

## Getting Started

This repository follows the Apache CloudStack development and build conventions. Before building or contributing, review:

- [INSTALL.md](INSTALL.md) for installation and environment requirements.
- [CONTRIBUTING.md](CONTRIBUTING.md) for contribution workflow and project conventions.

A Java and Maven development environment is required for the main platform modules. The web console and supporting tools may have additional dependencies described in their respective directories.

## Project Status

UOC is an evolving operations platform. Features, integrations, deployment profiles, and administrative workflows may change as the console is adapted to the environments it manages.

## License

This project retains the licensing and notices of the Apache CloudStack codebase. See [LICENSE](LICENSE) and [NOTICE](NOTICE) for details.


