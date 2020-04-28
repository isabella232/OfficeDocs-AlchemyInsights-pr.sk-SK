---
title: Pridanie skupiny na lokalitu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912981"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémy pri vytváraní skupiny pripojenej lokality SharePoint

1. Niektoré bežné problémy sa vyskytli pri vytváraní alebo opätovnom vytvorení skupiny pripojenej lokality.
Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou webovou adresou, musíte natrvalo odstrániť predchádzajúcu lokalitu.

   - Na stiahnutie [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Ďalšie informácie o Začíname s PowerShell, pozrite si Začíname [s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odstráňte lokalitu z odstránených lokalít pomocou rutiny cmdlet prostredia PowerShell [odstrániť SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell je potrebné natrvalo odstrániť skupiny lokalít.

1. Ak vytvárate skupinu pripojenú lokalitu a prijmete upozornenie: **Ďalšia skupina s rovnakým aliasom už existuje**, skontrolujte existujúce skupiny z [Microsoft 365 admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Ak chcete vyriešiť tento problém, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.

1. Existujú rôzne spôsoby vytvárania a používania moderných skupín so službou SharePoint.

   - Existujúce lokality môžete pripojiť k skupine Microsoft 365. Ďalšie informácie nájdete v téme [pripojenie skupiny Microsoft 365 pomocou používateľského rozhrania služby SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Ak chcete vytvoriť lokalitu Microsoft 365 Group Connected, musíte vytvoriť [tímovú lokalitu](https://admin.microsoft.com/sharepoint).
