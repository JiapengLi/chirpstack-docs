---
description: Adaptive data-rate reduces airtime and the device energy consumption.
---

# Adaptive data-rate (ADR)

Adaptive data-rate lets ChirpStack Network Server control the data-rate and
tx-power of the device, so that it uses less airtime and less power to
transmit the same amount of data. This is not only beneficial for the
energy consumtion of the device, but also optimizes the spectrum.

**Important:** ADR should only be used for static devices (devices that
do not move)!

## Activating ADR

The activation of ADR is controlled by the device. Only when the device
sends an uplink frame with the ADR flag set to `true` will ChirpStack Network Server
adjust the data-rate and tx-power of the device if needed.

## Configuration

To make sure there is enough link margin left after setting the ideal
data-rate and tx-power, it is important to configure the installation margin
correctly. See for more information [Configuration](../install/config.md).
