---
title: obj
description: Select object by name. Selects the specified vignette group by name and starts a new MSS.
solution: Experience Manager
feature: Dynamic Media Classic,SDK/API
role: Developer,User
exl-id: 17387203-f7a7-4876-a15b-2084894f981d
---
# obj{#obj}

Select object by name. Selects the specified vignette group by name and starts a new MSS.

 ` obj= *`name`*`

<table id="simpletable_6E0DA6CBCDCF4CDDAFA5A4C38E0D5FC5"> 
 <tr class="strow"> 
  <td class="stentry"> <p> <span class="codeph"> <span class="varname"> name </span> </span> </p> </td> 
  <td class="stentry"> <p>Group name or path/name. </p> </td> 
 </tr> 
</table>

Subgroups or individual objects may be selected using a fully qualified group path (i.e. by specifying the name of the target group or object preceded by all parent groups, separated by / (forward slashes).

If no group/object with the specified name is found, the action specified in `attribute::OnObjFail` is taken.

## Properties {#section-9463b36e8ff74c81a70c7c2b58927430}

Selection command; MSS delimiter. The object selection is persistent until another object is selected, either with `obj=` or `sel=`.

Group/object paths and names are case-insensitive.

## Default {#section-0c322850512c4896bb551856a549440e}

The first group in the vignette containing renderable objects is selected automatically when a new vignette is opened.

## See also {#section-d9d2c92ef48548f48b9781e2a8a5fb5a}

[sel=](../../../../../ir-api/http-protocol/image-rendering-api-ref/c-ir-http-protocol-ref/c-ir-http-protocol-command-reference/r-ir-sel.md#reference-01322c58d414481385c29fcdd27a090b), [attribute::OnFailObj](../../../../../ir-api/material-cat/image-rendering-api-ref/c-ir-material-catalog/c-ir-attributes-reference/r-ir-onfailobj.md#reference-4c6ba90418e84da5831f8573bbbf2c8d)
