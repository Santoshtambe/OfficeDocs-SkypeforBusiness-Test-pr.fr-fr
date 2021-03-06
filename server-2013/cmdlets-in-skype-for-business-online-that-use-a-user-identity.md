﻿---
title: Applets de commande utilisant l’identité d’un utilisateur
TOCTitle: Applets de commande utilisant l’identité d’un utilisateur
ms:assetid: be87409f-6372-4c70-91ac-6ef13dfbe65a
ms:mtpsurl: https://technet.microsoft.com/fr-fr/library/Dn362842(v=OCS.15)
ms:contentKeyID: 56269648
ms.date: 06/01/2017
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Applets de commande utilisant l’identité d’un utilisateur

 

_**Dernière rubrique modifiée :** 2015-06-22_

Dans Skype Entreprise Online, vous pouvez référencer l’identité d’un utilisateur individuel de différentes façons :

  - Vous pouvez utiliser le nom complet des services de domaine Active Directory de l’utilisateur. Par exemple :
    
        -Identity "Ken Myer"

  - Vous pouvez utiliser l’adresse SIP de l’utilisateur. Par exemple :
    
        -Identity "sip:kenmyer@litwareinc.com"

  - Vous pouvez utiliser le nom d’utilisateur principal de l’utilisateur. Par exemple :
    
        -Identity " kenmyer@litwareinc.com"

  - Vous pouvez utiliser le nom unique des services de domaine Active Directory de l’utilisateur. Par exemple :
    
        -Identity "CN=48ebd1ba-95d4-460c-b751-811ebf0c4611,OU=fa8226f5-14fa-46da-8 236-039b25bc7a27,OU=Lync Online Tenants,DC=litwareinc,DC=com"

Les applets de commande suivantes acceptent l’identité d’un utilisateur :

  - [Disable-CsMeetingRoom](disable-csmeetingroom.md)

  - [Enable-CsMeetingRoom](enable-csmeetingroom.md)

  - [Get-CsExUmContact](get-csexumcontact.md)

  - [Get-CsMeetingRoom](get-csmeetingroom.md)

  - [Get-CsOnlineUser](get-csonlineuser.md)

  - [Get-CsUserAcp](get-csuseracp.md)

  - [New-CsExUmContact](new-csexumcontact.md)

  - [Remove-CsExUmContact](remove-csexumcontact.md)

  - [Remove-CsUserAcp](remove-csuseracp.md)

  - [Set-CsExUmContact](set-csexumcontact.md)

  - [Set-CsMeetingRoom](set-csmeetingroom.md)

  - [Set-CsUserAcp](set-csuseracp.md)

Vous n’avez pas besoin de spécifier l’identité d’un utilisateur lorsque vous appelez une des applets de commande **Get-Cs**. Dans ce cas, les applets de commande retournent toutes les instances de l’élément spécifié. Par exemple, la commande suivante retourne des informations sur tous les utilisateurs activés pour Skype Entreprise Online :

    Get-CsOnlineUser

Le paramètre Identity est requis uniquement si vous voulez retourner des informations pour un utilisateur spécifique :

    Get-CsOnlineUser -Identity "Ken Myer"

## Voir aussi

#### Concepts

[Identités, étendues et clients](identities-scopes-and-tenants-in-skype-for-business-online.md)  
[Applets de commande de Lync Online](the-skype-for-business-online-cmdlets.md)

