---
title: IBidiSpl IBidiSpl SendRecv method
description: The IBidiSpl SendRecv method sends a bidi request to the printer.
ms.assetid: 0c91abd0-5e49-4e23-a50f-9d1dacf9d868
keywords: ["IBidiSpl SendRecv method Print Devices", "IBidiSpl SendRecv method Print Devices , IBidiSpl interface", "IBidiSpl interface Print Devices , IBidiSpl SendRecv method"]
topic_type:
- apiref
api_name:
- IBidiSpl.IBidiSpl SendRecv
api_location:
- bidispl.dll
api_type:
- COM
---

# IBidiSpl::IBidiSpl::SendRecv method


The **IBidiSpl::SendRecv** method sends a bidi request to the printer.

Syntax
------

```ManagedCPlusPlus
HRESULT IBidiSpl::SendRecv(
  [in] const LPCWSTR      pszAction,
  [in]       IBidiRequest *pRequest
);
```

Parameters
----------

*pszAction* \[in\]  
A pointer to a NULL-terminated string that specifies the action for this bidi request. It can be one of the following constants.

| Constant                          | Value              | Meaning                                                                                                            |
|-----------------------------------|--------------------|--------------------------------------------------------------------------------------------------------------------|
| BIDI\_ACTION\_ENUM\_SCHEMA        | L"EnumSchema"      | Enumerate the schema. The returned data will be a list of schema that the port monitor or print provider supports. |
| BIDI\_ACTION\_GET                 | L"Get"             | Get the value of a specified schema.                                                                               |
| BIDI\_ACTION\_GET\_ALL            | L"GetAll"          | Get the values of all child nodes of the specified schema.                                                         |
| BIDI\_ACTION\_SET                 | L"Set"             | Set a value of the schema.                                                                                         |
| BIDI\_ACTION\_GET\_WITH\_ARGUMENT | L"GetWithArgument" | Request the bidi schema value using the data set as input argument.                                                |

 

*pRequest* \[in\]  
A pointer to a single bidi request.

Return value
------------

The method returns one of the following values.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Value</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><strong>S_OK</strong></td>
<td align="left"><p>The operation was successfully carried out.</p></td>
</tr>
<tr class="even">
<td align="left"><strong>E_HANDLE</strong></td>
<td align="left"><p>The interface handle was invalid.</p></td>
</tr>
<tr class="odd">
<td align="left"><strong>None of the above</strong></td>
<td align="left"><p>The <strong>HRESULT</strong> contains an error code corresponding to the last error.</p></td>
</tr>
</tbody>
</table>

 

Note that the **HRESULT** may contain a system error code defined in [Bidi Error Codes](bidi-error-codes.md).

Remarks
-------

The BIDI\_ACTION\_\* values are case insensitive strings.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Target platform</p></td>
<td align="left"></td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">Bidispl.h</td>
</tr>
<tr class="odd">
<td align="left"><p>DLL</p></td>
<td align="left">Bidispl.dll</td>
</tr>
</tbody>
</table>

## See also


[**IBidiSpl**](ibidispl.md)

[Bidirectional Communication Interfaces](bidirectional-communication-interfaces.md)

[Bidirectional Communication Schema](bidirectional-communication-schema.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bprint\print%5D:%20IBidiSpl::IBidiSpl::SendRecv%20method%20%20RELEASE:%20%283/29/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





