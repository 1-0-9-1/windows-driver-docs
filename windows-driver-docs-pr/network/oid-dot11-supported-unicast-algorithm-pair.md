---
title: OID_DOT11_SUPPORTED_UNICAST_ALGORITHM_PAIR
author: windows-driver-content
description: OID_DOT11_SUPPORTED_UNICAST_ALGORITHM_PAIR
ms.assetid: 8b16dfca-d9f3-4b51-8363-2799b8fb49c7
ms.author: windowsdriverdev
ms.date: 08/08/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
keywords: 
 -OID_DOT11_SUPPORTED_UNICAST_ALGORITHM_PAIR Network Drivers Starting with Windows Vista
---

# OID\_DOT11\_SUPPORTED\_UNICAST\_ALGORITHM\_PAIR


**Important**  The [Native 802.11 Wireless LAN](https://msdn.microsoft.com/library/windows/hardware/ff560690) interface is deprecated in Windows 10 and later. Please use the WLAN Device Driver Interface (WDI) instead. For more information about WDI, see [WLAN Universal Windows driver model](https://msdn.microsoft.com/library/windows/hardware/dn897672).

 

When queried, the OID\_DOT11\_SUPPORTED\_UNICAST\_ALGORITHM\_PAIR object identifier (OID) requests that the miniport driver return a list of the 802.11 authentication and cipher algorithms that the 802.11 station supports for unicast packets.

The data type for this OID is the [**DOT11\_AUTH\_CIPHER\_PAIR\_LIST**](https://msdn.microsoft.com/library/windows/hardware/ff547662) structure.

When OID\_DOT11\_SUPPORTED\_UNICAST\_ALGORITHM\_PAIR is queried, the miniport driver only returns 802.11 authentication and cipher algorithms that the 802.11 station supports for the current value of the IEEE **dot11DesiredBSSType** management information base (MIB) object. For more information about this MIB object, see [OID\_DOT11\_DESIRED\_BSS\_TYPE](oid-dot11-desired-bss-type.md).

**Note**  For each value of the **dot11DesiredBSSType** MIB object, the miniport driver must not change the list of the 802.11 authentication and cipher algorithms after the OID\_DOT11\_SUPPORTED\_UNICAST\_ALGORITHM\_PAIR is queried.

 

There must be at least one cipher algorithm defined for each supported authentication algorithm. If the miniport driver does not support any unicast cipher algorithms for a particular authentication algorithm, it must still create a list entry for the authentication algorithm and use **DOT11\_CIPHER\_ALGO\_NONE** for the related cipher algorithm.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Version</p></td>
<td><p>Available in Windows Vista and later versions of the Windows operating systems.</p></td>
</tr>
<tr class="even">
<td><p>Header</p></td>
<td>Windot11.h (include Ndis.h)</td>
</tr>
</tbody>
</table>

## See also


[Native 802.11 Wireless LAN OIDs](https://msdn.microsoft.com/library/windows/hardware/ff560691)

 

 




