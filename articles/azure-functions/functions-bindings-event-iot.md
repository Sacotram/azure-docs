---
title: Azure IoT Hub bindings for Azure Functions
description: Learn to use IoT Hub trigger and binding in Azure Functions.
ms.topic: reference
ms.date: 03/04/2022
zone_pivot_groups: programming-languages-set-functions-lang-workers
---

# Azure IoT Hub bindings for Azure Functions

This set of articles explains how to work with Azure Functions bindings for IoT Hub. The IoT Hub support is based on the [Azure Event Hubs Binding](functions-bindings-event-hubs.md).

> [!IMPORTANT]
> While the following code samples use the Event Hub API, the given syntax is applicable for IoT Hub functions.

| Action | Type |
|--------|------|
| Respond to events sent to an IoT hub event stream. | [Trigger](./functions-bindings-event-iot-trigger.md) |

[!INCLUDE [functions-bindings-event-hubs](../../includes/functions-bindings-event-hubs.md)]

##Connections
The connection property is a reference to environment configuration that contains name of an application setting containing a connection string. For an IoT Hub trigger, the connection string is available in Built-in endpoints menu of the IoT Hub under the name of Event Hub-compatible endpoint. (https://learn.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-read-builtin).  The connection string should be edited to remove the EntityPath if this property is already added as an attribute in the trigger.

## Next steps

- [Respond to events sent to an event hub event stream (Trigger)](./functions-bindings-event-iot-trigger.md)
- [Write events to an event stream (Output binding)](./functions-bindings-event-iot-output.md)
