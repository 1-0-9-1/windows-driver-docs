---
title: NetRxQueueInitAddPacketContextAttributes method
description: NetRxQueueInitAddPacketContextAttributes method
ms.assetid: ED6DC974-6110-4651-973D-4AAF2A148E9B
keywords:
- WDF Network Adapter Class Extension NetRxQueueInitAddPacketContextAttributes, NetAdapterCx NetRxQueueInitAddPacketContextAttributes, NetCx NetRxQueueInitAddPacketContextAttributes
ms.author: windowsdriverdev
ms.date: 09/06/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# NetRxQueueInitAddPacketContextAttributes method

[!include[NetAdapterCx Beta Prerelease](../netcx-beta-prerelease.md)]

The **NetRxQueueInitAddPacketContextAttributes** method adds an initialized [NET_PACKET_CONTEXT_ATTRIBUTES](net-packet-context-attributes.md) structure to a receive queue's packet context space.

## Syntax

```cpp
NTSTATUS FORCEINLINE NetRxQueueInitAddPacketContextAttributes(
    _Inout_ PNETRXQUEUE_INIT                NetRxQueueInit,
    _In_    PNET_PACKET_CONTEXT_ATTRIBUTES  PacketContextAttributes
);
```

## Parameters

*NetRxQueueInit* [in, out]  
A pointer to the **NETRXQUEUE_INIT** structure that the client driver received in [*EVT_NET_ADAPTER_CREATE_RXQUEUE*](evt-net-adapter-create-rxqueue.md).

*PacketContextAttributes* [in]  
A pointer to an initialized [NET_PACKET_CONTEXT_ATTRIBUTES](net-packet-context-attributes.md) structure that represents attributes for the context space of each [NET_PACKET](net-packet.md) in this queue.

## Return value

If the operation is successful, this method returns STATUS_SUCCESS. Otherwise, an appropriate [NTSTATUS](https://msdn.microsoft.com/library/windows/hardware/ff557697) error code.

## Remarks

The NETRXQUEUE_INIT structure is an opaque structure that is defined and allocated by NetAdapterCx, similar to WDFDEVICE_INIT. The client driver receives a pointer to the NETRXQUEUE_INIT object in its [*EVT_NET_ADAPTER_CREATE_RXQUEUE*](evt-net-adapter-create-rxqueue.md) callback function, where this method is called to add context attributes to the queue for each packet context context the driver has created.

## Requirements

|     |     |
| --- | --- |
| Target platform | Universal |
| Minimum KMDF version | 1.23 |
| Minimum NetAdapterCx version | 1.1 |
| Header | Netrxqueue.h (include NetAdapterCx.h) |
| IRQL | PASSIVE_LEVEL |

