---
title: SENSOR\_CATEGORY\_ALL
description: The SENSOR\_CATEGORY\_ALL category represents the set of all platform-defined sensor categories.
ms.assetid: 9a4524d2-055c-46e0-9650-66e6f2872fbc
keywords: ["SENSOR_CATEGORY_ALL Sensor Devices"]
topic_type:
- apiref
api_name:
- SENSOR_CATEGORY_ALL
api_location:
- Sensors.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 01/04/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# SENSOR\_CATEGORY\_ALL


The SENSOR\_CATEGORY\_ALL category represents the set of all platform-defined sensor categories.

### <span id="platform_defined_property_keys"></span><span id="PLATFORM_DEFINED_PROPERTY_KEYS"></span>Platform-defined Property Keys

This category includes the following platform-defined data fields.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Data type</th>
<th>Type</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>SENSOR_DATA_TYPE_TIMESTAMP</p></td>
<td><p><strong>VT_FILETIME</strong></p></td>
<td><p>Required for all data reports. Marks each data report with the time the data report was created. Use Universal Coordinated Time (UTC).</p></td>
</tr>
</tbody>
</table>

 

**Important**   Each platform-defined common data type **PROPERTYKEY** is based on a common **GUID** that is named SENSOR\_DATA\_TYPE\_COMMON\_GUID. As it is a reserved base value, do not use this **GUID** to define your own property keys.

 

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum supported client</p></td>
<td><p>Windows 7</p></td>
</tr>
<tr class="even">
<td><p>Minimum supported server</p></td>
<td><p>None supported</p></td>
</tr>
<tr class="odd">
<td><p>Version</p></td>
<td><p>Available in Windows 7.</p></td>
</tr>
<tr class="even">
<td><p>Header</p></td>
<td>Sensors.h</td>
</tr>
</tbody>
</table>

 

 





