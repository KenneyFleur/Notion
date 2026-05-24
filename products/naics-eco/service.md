---
title: NAICS Economy — Service Tier Deployment Guide
sku: NAICS-ECO
tier: Professional
price: $197
entity: Volactic LLC
prepared_by: Kenney Edward Belliard Fleurimond
version: "1.0"
classification: Service Deployment Reference
---

> **NOTICE: This service tier is NOT included in the one-time deliverable purchase.**  
> It is available as a separate enterprise licensing engagement. Contact Volactic LLC to provision.

# NAICS Economy — Service Tier

## SKU: NAICS-ECO | Tier: Professional | One-Time Deliverable Price: $197

## What This Is

This document describes the **service-tier deployment** available as a separate engagement: the customer provisions their own Replit workspace, runs Volactic-provided agent code, and communicates with the VSMA Codex Platform via authenticated BaaS API endpoints.

## Customer Responsibilities

- Create and fund their own Replit account
- Deploy the provided agent scaffolding on their Replit workspace
- Pay Replit directly for all compute, storage, and egress charges
- Maintain their own API keys (OpenAI, Notion, GitHub, etc.)
- Manage uptime, monitoring, and backups on their infrastructure

## Volactic Provides

- Customer-managed NAICS sector crawler on their own Replit workspace
- Volactic provides: crawler code, NAICS data feed spec, sector expansion templates
- Customer provisions: Replit account, scheduled crawler deployment, API keys
- Customer pays Replit directly for all compute and storage
- Customer crawler pushes sector updates to Volactic mesh via authenticated BaaS endpoint
- 20-sector expansion runs on customer infrastructure; zero Volactic compute cost

## BaaS API Connection (Hard Limits)

- Endpoint: `POST /api/public/braid-analyze`
- Authentication: BaaS API key (provided per service license)
- Rate limit: **60 requests/minute per key**
- Daily cap: **2,000 requests/day per key**
- Max payload size: **100 KB per request**
- Max webhooks/minute: **30 per tenant**
- Data retention window: **90 days** on Volactic mesh; customer retains primary copy
- Max concurrent tenants per license: **1**
- Support scope: Integration protocol + compatibility updates only; customer-managed infrastructure support is customer responsibility

## Billing Separation

| Cost Item | Paid By |
|-----------|---------|
| Replit compute + storage | Customer |
| OpenAI LLM tokens (if applicable) | Customer |
| External API calls (USPTO, Grants.gov, etc.) | Customer |
| Volactic BaaS API access | Included in service license |
| Volactic mesh sync | Included in service license |

## Support

- Entity: Volactic LLC
- Sovereign governance: VSMA Codex Platform
- Patents: USPTO 19/414,612, 19/392,097, 73057906
- For service-tier licensing inquiries: Contact Volactic LLC

---

> This service-tier deployment is governed under the VSMA Sovereign IP Continuity System. Customer-managed infrastructure remains customer property. Volactic retains IP and governance protocol rights.
