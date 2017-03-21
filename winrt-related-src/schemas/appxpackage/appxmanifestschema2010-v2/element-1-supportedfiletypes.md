---
Description: Defines the file types that the app can share.
Search.Product: eADQiWindows 10XVcnh
title: 'SupportedFileTypes (type: CT_CharmsSupportedFileTypes)'
ms.assetid: f5706357-708f-4d3e-bbca-15272e6b77dc
author: laurenhughes
ms.author: lahugh
keywords: windows 10, uwp, schema, package manifest
---

# SupportedFileTypes (type: CT_CharmsSupportedFileTypes)




Defines the file types that the app can share.

## Element hierarchy

<dl>
<dt><a href="element-extension.md">&lt;Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-sharetarget.md">&lt;ShareTarget&gt;</a></dt>
<dd><b>&lt;SupportedFileTypes&gt;</b></dd>
</dl>
<dl>
<dt><a href="element-fileopenpicker.md">&lt;FileOpenPicker&gt;</a></dt>
<dd><b>&lt;SupportedFileTypes&gt;</b></dd>
</dl>
<dl>
<dt><a href="element-filesavepicker.md">&lt;FileSavePicker&gt;</a></dt>
<dd><b>&lt;SupportedFileTypes&gt;</b></dd>
</dl>
</dd>
</dl>
## Syntax

``` syntax
<SupportedFileTypes>

  <!-- Child elements -->
  ( FileType{1,10000}
  | SupportsAnyFileType
  )

</SupportedFileTypes>
```

### Key

`{}`   specific range of occurrences

## Attributes and Elements


### Attributes

None.

### Child Elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Child Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[FileType (type: ST_FileType)](element-1-filetype.md)</td>
<td><p>A file type specified as its file type extension. It is unique per application in the package and is case sensitive.</p></td>
</tr>
<tr class="even">
<td>[SupportsAnyFileType](element-supportsanyfiletype.md)</td>
<td><p>Indicates whether all file types are supported for sharing.</p></td>
</tr>
</tbody>
</table>

 

### Parent Elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parent Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[FileOpenPicker](element-fileopenpicker.md)</td>
<td><p>Declares an app extensibility point of type <strong>windows.fileOpenPicker</strong>. The app lets the user choose and open the specified types of files.</p></td>
</tr>
<tr class="even">
<td>[FileSavePicker](element-filesavepicker.md)</td>
<td><p>Declares an app extensibility point of type <strong>windows.fileSavePicker</strong>. The app lets the user choose the file name, extension, and storage location for the specified types of files.</p></td>
</tr>
<tr class="odd">
<td>[ShareTarget](element-sharetarget.md)</td>
<td><p>Declares an app extension point of type <strong>windows.shareTarget</strong>. The app can share the specified types of files.</p></td>
</tr>
</tbody>
</table>

 

## Related elements


The following elements have the same name as this one, but different content or attributes:

-   **[SupportedFileTypes (type: CT_FTASupportedFileTypes)](element-supportedfiletypes.md)**

## Examples

```XAML
<SupportedFileTypes>
  <FileType>.txt</FileType>
  <FileType>.docx</FileType>
</SupportedFileTypes>
```

## Requirements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Namespace</p></td>
<td><p>http://schemas.microsoft.com/appx/2010/manifest</p></td>
</tr>
</tbody>
</table>

 

 


