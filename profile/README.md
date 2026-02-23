<div align="center">

# ABRAK
### Identity and Event Center for the Holding Ecosystem

<p>
  <img alt="Org" src="https://img.shields.io/badge/Org-abrakorg-c3b97f?style=for-the-badge">
  <img alt="Model" src="https://img.shields.io/badge/Model-Identity%20%26%20Events-0f1f38?style=for-the-badge">
  <img alt="Status" src="https://img.shields.io/badge/Status-Operational-2e7d32?style=for-the-badge">
</p>

</div>

## About Abrak
Abrak is the central governance layer for:
- identity and access
- plans, licenses, entitlements
- usage and event collection
- central commands to connected services
- billing and audit orchestration

## Core Repositories
- `ABRAK_CO_DATACENTER` - governance, registry, standards, safe ops documentation
- `filament-3` - Abrak Hub (Filament)
- `odoo-v2` - CRM/ERP Odoo service line
- `abrak-connector-php` - PHP connector contract scaffold
- `abrak-connector-python` - Python connector contract scaffold

## Engineering Rules (Short)
- No direct operational action on `PC.HAIDA.CO`
- No direct operational action on `CRM.HAIDA.CO`
- Repository-first changes must be reversible and documented
- Hub and Odoo remain integrated under a single platform model

## Developer Start (VS Code Tunnel)
Use the server-side workspace and shell shortcuts after tunnel login:
- Workspace: `/root/work/abrakorg.code-workspace`
- Core repos: `/root/work/*`, `/root/odoo-v2`

## Language
- Persian-first operational context
- English-compatible engineering documentation
