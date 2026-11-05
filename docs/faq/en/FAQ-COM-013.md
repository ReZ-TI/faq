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
  - https://support.apple.com/en-ie/102078
---

# FAQ-COM-013 · Do Matter over Thread devices need a gateway?

> Draft pending review. Not published to the website.

## Answer

It depends on whether the site already has a compatible Thread border router — it is not only about our device. A Matter over Thread device needs a Thread border router supported by the ecosystem it joins: if the site already has a compatible Apple home hub or a compatible border router, that can be reused and no vendor gateway from us is needed; if the site only has Thread bulbs and the phone itself does not support Thread, the device cannot be joined. On Apple platforms the model also matters: only certain Thread-capable Apple devices can pair and control locally, while automation and remote access still require a home hub such as a HomePod, an Apple TV or a compatible border router. Tell us the hub or border router already on site, the phone model and the control platform, and we can confirm whether anything needs to be added. If Tuya Zigbee versions are used as well, we recommend adding a Home Assistant host with a Zigbee gateway for unified control.

## Scope

Models supporting Matter over Thread. Whether a vendor gateway can be skipped depends on the ecosystem on site, the phone model and the existing border router; this does not imply that all products work without a gateway in any environment.

## Basis and open items (internal verification, not published with the answer)

- Basis (public): Apple support article on adding accessories from a mobile device <https://support.apple.com/en-ie/102078> (Thread-capable model requirements; local pairing versus hub-dependent automation and remote access).
- Basis (restricted): internal evidence ledger **FAQ-EVID-2026-11-05 §3** — October 2026 outbound position (Matter over Thread joins Apple Home directly; Tuya Zigbee needs a Home Assistant host plus Zigbee gateway), not published here.
- Open: whether schedules run on-device or in the app varies by model; whether a border router is included with an order needs product-line confirmation.

[Chinese version](../zh-CN/FAQ-COM-013.md) · [Index](README.md)
