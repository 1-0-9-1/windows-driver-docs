---
title: SENSOR\_CATEGORY\_BIOMETRIC
description: The SENSOR\_CATEGORY\_BIOMETRIC category contains sensors that provide information about living beings.
ms.assetid: e26073e1-11cc-40a9-9a60-3a15ceb46059
keywords: ["SENSOR_CATEGORY_BIOMETRIC Sensor Devices"]
topic_type:
- apiref
api_name:
- SENSOR_CATEGORY_BIOMETRIC
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

# SENSOR\_CATEGORY\_BIOMETRIC


The SENSOR\_CATEGORY\_BIOMETRIC category contains sensors that provide information about living beings.

### <span id="platform_defined_sensor_types"></span><span id="PLATFORM_DEFINED_SENSOR_TYPES"></span>Platform-defined Sensor Types

This category includes the following platform-defined sensor types.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Sensor type</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>SENSOR_TYPE_HUMAN_PRESENCE</p></td>
<td><p>Sensors that detect human presence.</p></td>
</tr>
<tr class="even">
<td><p>SENSOR_TYPE_HUMAN_PROXIMITY</p></td>
<td><p>Sensors that detect human proximity.</p></td>
</tr>
<tr class="odd">
<td><p>SENSOR_TYPE_TOUCH</p></td>
<td><p>Touch sensors.</p></td>
</tr>
</tbody>
</table>

 

### <span id="platform_defined_data_fields"></span><span id="PLATFORM_DEFINED_DATA_FIELDS"></span>Platform-defined Data Fields

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
<td><p>SENSOR_DATA_TYPE_HUMAN_PRESENCE</p></td>
<td><p><strong>VT_BOOL</strong></p></td>
<td><p><strong>VARIANT_TRUE</strong> when a human is using the computer.</p></td>
</tr>
<tr class="even">
<td><p>SENSOR_DATA_TYPE_HUMAN_PROXIMITY_METERS</p></td>
<td><p><strong>VT_R4</strong></p></td>
<td><p>Distance between a human and the computer, in meters.</p></td>
</tr>
<tr class="odd">
<td><p>SENSOR_DATA_TYPE_TOUCH_STATE</p></td>
<td><p><strong>VT_BOOL</strong></p></td>
<td><p><strong>VARIANT_TRUE</strong> when the touch sensor is being touched, otherwise <strong>VARIANT_FALSE</strong>.</p></td>
</tr>
</tbody>
</table>

 

**Important**   Each platform-defined biometric data type **PROPERTYKEY** is based on a common **GUID** that is named SENSOR\_DATA\_TYPE\_BIOMETRIC\_GUID. As it is a reserved base value, do not use this **GUID** to define your own property keys.

 

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

 

 





