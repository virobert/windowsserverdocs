---
title: get-AllDriverGroups
description: Reference article for get-AllDriverGroups, which displays information about all the driver groups on a server.
ms.topic: reference
ms.assetid: f245ba53-f150-41b1-8418-38dcf0410a05
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---
# get-AllDriverGroups

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Displays information about all the driver groups on a server.

## Syntax
```
wdsutil /Get-AllDriverGroups [/Server:<Server name>] [/Show:{PackageMetaData | Filters | All}]
```
### Parameters
|Parameter|Description|
|-------|--------|
|[/Server:<Server name>]|Specifies the name of the server. This can be the NetBIOS name or the FQDN. If a server name is not specified, the local server is used.|
|[/Show: {PackageMetaData &#124; Filters &#124; All}]|Displays the metadata for all the driver packages in the specified group. **PackageMetaData** displays information about all the filters for the driver group. **Filters** displays the metadata for all driver packages and filters for the group.|
## Examples
To view information about a driver file, type:
```
wdsutil /Get-AllDriverGroups /Server:MyWdsServer /Show:All
```
```
wdsutil /Get-AllDriverGroups [/Show:PackageMetaData]
```
## Additional References
- [Command-Line Syntax Key](command-line-syntax-key.md)
[Using the get-DriverGroup Command](using-the-get-drivergroup-command.md)
