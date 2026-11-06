---
id: FAQ-COM-013
locale: en
status: approved
audience: public_candidate
owner: kelvinchen1119
reviewed_by: kelvinchen1119
reviewed_at: 2026-11-06
---

# FAQ-COM-013 · Do Matter over Thread devices need a gateway?

## Answer

It depends on whether the site already has a compatible Thread border router — it is not only about our device. A Matter over Thread device needs a Thread border router supported by the ecosystem it joins: if the site already has a compatible Apple home hub or a compatible border router, that can be reused and no vendor gateway from us is needed; if the site only has Thread bulbs and the phone itself does not support Thread, the device cannot be joined. On Apple platforms the model also matters: only certain Thread-capable Apple devices can pair and control locally, while automation and remote access still require a home hub such as a HomePod, an Apple TV or a compatible border router. Tell us the hub or border router already on site, the phone model and the control platform, and we can confirm whether anything needs to be added.

For Tuya, use a compatible Tuya gateway that supports Matter over Thread and the relevant device types.

If you also use Tuya Zigbee devices, we recommend adding a Home Assistant host together with our Thread Dongle for unified control. The Thread Dongle provides the Matter over Thread connection; Zigbee devices connect through a Zigbee gateway or coordinator compatible with Home Assistant. Our sales team will confirm the required setup based on your existing devices. See [FAQ-COM-012](FAQ-COM-012.md) for the distinction between the protocols and Tuya connectivity.

## Scope

Models supporting Matter over Thread. Whether a vendor gateway can be skipped depends on the ecosystem on site, the phone model and the existing border router; this does not imply that all products work without a gateway in any environment.

[中文](../zh-CN/FAQ-COM-013.md) · [Index](README.md)
