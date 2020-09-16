---
title: Pridanie skupiny na lokalitu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771223"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémy pri vytváraní skupiny pripojenej lokality v SharePointe

1. Niektoré bežné problémy, ktoré sa vyskytli pri vytváraní alebo opätovnom vytvorení lokality pripojenej k skupine.
Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou URL adresou, budete musieť predchádzajúcu lokalitu odstrániť natrvalo.

   - Stiahnuť [prostredie spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Ďalšie informácie o tom, ako začať pracovať s prostredím PowerShell, nájdete v téme Začíname [pracovať so službou SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odstránenie lokality z odstránených lokalít pomocou rutiny typu cmdlet prostredia na [Odstránenie SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . Na trvalé odstránenie skupinových lokalít sa vyžaduje prostredie PowerShell.

1. Ak vytvárate lokalitu pripojenú ku skupine a zobrazíte upozornenie: **Ďalšia skupina s rovnakým aliasom už existuje**, pozrite si existujúce skupiny z [centra spravovania služby Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Ak chcete problém vyriešiť, odstráňte existujúcu skupinu, ak ju už nepotrebujete, alebo vytvorte lokalitu s iným priradeným aliasom.

1. Existujú rôzne spôsoby na vytváranie a používanie moderných skupín v SharePointe.

   - Existujúce lokality môžete pripojiť k skupine Microsoft 365. Ďalšie informácie nájdete v téme [pripojenie skupiny Microsoft 365 pomocou používateľského rozhrania služby SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Ak chcete vytvoriť lokalitu pripojenú ku skupine Microsoft 365, budete musieť vytvoriť [tímovú lokalitu](https://admin.microsoft.com/sharepoint).
