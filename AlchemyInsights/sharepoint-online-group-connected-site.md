---
title: Pridanie skupiny na SharePoint lokalitu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318139"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Bežné problémy pri vytváraní lokality pripojenej ku skupine v SharePoint

1. Ak ste odstránili skupinu a pripojenú lokalitu a chcete vytvoriť ďalšiu lokalitu s rovnakou URL adresou, budete musieť predchádzajúcu lokalitu natrvalo odstrániť.

   - Stiahnuť [prostredie správy SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Ďalšie informácie o tom, ako začať pracovať s prostredím PowerShell, nájdete v téme [Začíname pracovať s prostredím SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Odstráňte lokalitu z odstránených lokalít pomocou rutiny typu cmdlet prostredia Powershell [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Na trvalé odstránenie skupinových lokalít sa vyžaduje prostredie PowerShell.

1. Ak vytvárate pripojenú lokalitu skupiny a zobrazí sa upozornenie: Iná skupina s rovnakým **aliasom** už existuje, skontrolujte existujúce skupiny z [Centrum spravovania služby Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Ak chcete tento problém vyriešiť, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.

1. Existujú rôzne spôsoby, ako vytvoriť a používať moderné skupiny s SharePoint.

   - Môžete pripojiť existujúce lokality k Microsoft 365 skupine. Ďalšie informácie nájdete v [Pripojenie skupiny Microsoft 365 pomocou používateľského SharePoint rozhrania](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Ak chcete Microsoft 365 pripojenú ku skupine, musíte vytvoriť [tímovú lokalitu.](https://admin.microsoft.com/sharepoint)
