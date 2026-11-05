---
id: FAQ-COM-013
locale: en
status: draft
audience: public_candidate
owner: kelvinchen1119
evidence_checked_on: 2026-11-05
reviewed_by: null
reviewed_at: null
sources:
  - ../sources/README.md
---

# FAQ-COM-013 · Do Matter over Thread devices need a gateway?

> Draft pending review. Not published to the website.

## Answer

Devices supporting Matter over Thread can join ecosystems such as Apple Home directly. No vendor gateway is required and no cloud dependency is involved. If the site also runs Tuya Zigbee versions, we recommend one Home Assistant host plus a Zigbee gateway so both types are controlled from one interface. Whether an additional Thread border router is needed depends on the Thread devices and network coverage already on site — send us a floor plan or device list and we can confirm together.

## Scope

Models supporting Matter over Thread. This does not imply that all products work without a gateway.

## Basis and open items (internal verification, not published with the answer)

- Basis: [Sources and confirmed business rules](../sources/README.md).
- Open: whether schedules run on-device or in the app varies by model; whether a border router is included with the order needs confirmation from the product line.

[中文版本](../zh-CN/FAQ-COM-013.md) · [Index](README.md)
