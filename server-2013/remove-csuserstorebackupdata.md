﻿---
title: Remove-CsUserStoreBackupData
TOCTitle: Remove-CsUserStoreBackupData
ms:assetid: 71c8e8ee-61c7-4737-bdac-8cfc80bac126
ms:mtpsurl: https://technet.microsoft.com/fr-fr/library/JJ205003(v=OCS.15)
ms:contentKeyID: 49297691
ms.date: 05/20/2016
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Remove-CsUserStoreBackupData

 

_**Dernière rubrique modifiée :** 2015-03-09_

Removes outdated information from the specified user store. "Outdated information" refers user data from a Registrar pool no longer paired with the specified user store. For example, suppose Pools A and B were once paired; now, however, that association has been changed, and Pools A and C are paired. When run against Pool A, the Remove-CsUserStoreBackupData cmdlet will remove information about users from Pool B. Cette applet de commande est une nouveauté de Lync Server 2013.

## Syntaxe

    Remove-CsUserStoreBackupData -PoolFqdn <Fqdn> [-Confirm [<SwitchParameter>]] [-Force <SwitchParameter>] [-WhatIf [<SwitchParameter>]]

## Examples

## Example 1

The command shown in Example 1 removes outdated user store information stored by the pool atl-cs-001.litwareinc.com and its associated backup pool.

    Remove-CsUserStoreBackupData -PoolFqdn "atl-cs-001.litwareinc.com"

## Detailed Description

Lync Server 2013 enables you to associate a pair of pools. When you do this, each pool maintains two sets of user information: information about the users homed on the pool in question and information about the users homed on the associated pool. Maintaining both sets of user information allows Pool B to register and service the users from Pool A should Pool A need to be failed over.

If you later change the association between these two pools, the "extra" user data is not automatically deleted from the two pools; for example, Pool A will continue to store user data for Pool B. (However, this data will no longer be updated and replicated.) The **Remove-CsUserStoreBackupData** cmdlet enables you to delete the data from Pool B that is no longer needed on Pool A.

To return a list of all the role-based access control (RBAC) roles this cmdlet has been assigned to (including any custom RBAC roles you have created yourself), run the following command from the Windows PowerShell prompt:

Get-CsAdminRole | Where-Object {$\_.Cmdlets –match "Remove-CsUserStoreBackupData"}

**Panneau de configuration Lync Server:** The functions carried out by the **Remove-CsUserStoreBackupData** cmdlet are not available in the Panneau de configuration Lync Server.

## Paramètres


<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Required</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><em>PoolFqdn</em></p></td>
<td><p>Required</p></td>
<td><p>Microsoft.Rtc.Management.Deploy.Fqdn</p></td>
<td><p>Fully qualified domain name of the pool where &quot;outdated&quot; user information should be removed. For example:</p>
<p>–PoolFqdn &quot;atl-cs-001.litwareinc.com&quot;</p></td>
</tr>
<tr class="even">
<td><p><em>Confirm</em></p></td>
<td><p>Optional</p></td>
<td><p>System.Management.Automation.SwitchParameter</p></td>
<td><p>Prompts you for confirmation before executing the command.</p></td>
</tr>
<tr class="odd">
<td><p><em>Force</em></p></td>
<td><p>Optional</p></td>
<td><p>System.Management.Automation.SwitchParameter</p></td>
<td><p>Suppresses the display of any non-fatal error message that might arise when running the command.</p></td>
</tr>
<tr class="even">
<td><p><em>WhatIf</em></p></td>
<td><p>Optional</p></td>
<td><p>System.Management.Automation.SwitchParameter</p></td>
<td><p>Describes what would happen if you executed the command without actually executing the command.</p></td>
</tr>
</tbody>
</table>


## Input Types

None. The **Remove-CsUserStoreBackupData** cmdlet does not accept pipelined input.

## Return Types

None.

## Voir aussi

#### Autres ressources

[Get-CsBackupServiceStatus](get-csbackupservicestatus.md)

