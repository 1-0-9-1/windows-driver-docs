---
title: Marshalling helper functions
description: This topic provides information about the marshaling helper functions in the sensorsutils.h header file.
ms.assetid: AE5C70E4-1971-4BAF-AE7D-315A15F030DD
ms.author: windowsdriverdev
ms.date: 01/04/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Marshalling helper functions


This topic provides information about the marshaling helper functions in the *sensorsutils.h* header file.

These helper functions are used by the v2 sensor drivers, and they're used along with the sensor device driver software interface (DDSI).

If you implement your own marshaling helper functions, remember that helper functions must not be used when populating the enumeration list in the [**SENSOR\_CONFIG**](https://msdn.microsoft.com/library/windows/hardware/dn957096) structure, or when reporting updated data with the [**SensorsCxSensorDataReady**](https://msdn.microsoft.com/library/windows/hardware/dn957088) function.

## <span id="in_this_section"></span>In this section


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Topic</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[Time stamp helper](timestamp-helper.md)</p></td>
<td><p>The time stamp helper function is used by v2 sensor drivers, and it's used with the sensor device driver software interface (DDSI).</p></td>
</tr>
<tr class="even">
<td><p>[PropVariant helpers](propvariant-helpers.md)</p></td>
<td><p>The PropVariant helper functions are used by the v2 sensor drivers for manipulating the [PROPVARIANT](https://msdn.microsoft.com/library/windows/desktop/aa380072.aspx) structures associated with the sensors.</p></td>
</tr>
<tr class="odd">
<td><p>[Collection list helpers](collection-list-helpers.md)</p></td>
<td><p>The collection list helper functions are used by the v2 sensor drivers, for working with [<strong>SENSOR_COLLECTION_LIST</strong>](https://msdn.microsoft.com/library/windows/hardware/dn957092) structures.</p></td>
</tr>
<tr class="even">
<td><p>[Collection list serialization helpers](collection-list-serialization-helpers.md)</p></td>
<td><p>The collection list serialization helper functions are used by the v2 sensor drivers, for performing serialization-related operations on [<strong>SENSOR_COLLECTION_LIST</strong>](https://msdn.microsoft.com/library/windows/hardware/dn957092) structures.</p></td>
</tr>
<tr class="odd">
<td><p>[Collection list legacy helpers](collection-list-legacy-helpers.md)</p></td>
<td><p>The collection list legacy helper functions are used by v2 sensor drivers for interacting with [<strong>SENSOR_COLLECTION_LIST</strong>](https://msdn.microsoft.com/library/windows/hardware/dn957092) structures.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Requirements"></span><span id="requirements"></span><span id="REQUIREMENTS"></span>Requirements


**Header:** Sensorsutils.h

 

 





